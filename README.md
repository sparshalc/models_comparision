# Bank Table
Missing: address,contact_no,creator_id,updater_id

# Group Table
Missing: name,
Default: false missing for for_trial_balance

# Bank Accounts
Additional Attributes: bank_branch,address,contact_no

# Vendor Accounts
Missing: branch_id

# Cheque Entries
reference with client_account, branch

Default: 0 missing for print_status, cheque_issued_type, status

precision: 15, scale: 4, default: 0.00 (amount)

Additional: fy_code

# fms_ledgers
Additional: restricted(booelan)

Missing: name, cliend_code, opening_blnc, closing_blnc, branch_id, dr_amount, cr_amount, client_account, employee_account

# Ledgers Balances
Missing: creator_id,updater_id,branch_id

precision: 15, scale: 4, default: 0.00 (opening_balance,closing_balance,dr_amount,cr_amount)

Additional: opening_balance_type

# Vouchers
Missing: date_bs,desc,beneficiary_name,

Missing enum default values for voucher_type and voucher_status

Additional: value_date

# Particulars
Missing: opening_balance, cheque_number, name, description,running_blnc, date_bs,branch_id

Missing Default Value for ledger_type, particular_status

missing precision: 15, scale: 4, default: 0 for amount

Additional: value_date

# Settlements
Missing: name, date_bs, description,receiver_name, 

Additional: settlement_by_cheque_type,cash_amount,belongs_to_batch_payment,date

# Cheque Entry Particular Associations
Additional: amount

# ParticularSettlementAssociations
Missing Default Value for association_type
