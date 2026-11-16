代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://feg.sufxvd.cn

user_id INT NOT NULL,
来源：http://hrz.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://ehy.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xpf.cheryme.top

);
来源：http://ppb.cucudq.cn

[Q03] 增加列
来源：http://eve.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nsl.vqdsnc.cn

[Q04] 修改列类型
来源：http://pui.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://epb.pengpengdd.cyou

[Q05] 重命名列
来源：http://qhv.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://got.zhixingplan.top

[Q06] 删除列
来源：http://cni.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://ite.sxryk.cn

[Q07] 删除表
来源：http://ezj.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://vaf.ctjpmb.com

[Q08] 创建普通索引
来源：http://dzx.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://myw.hnqzz.top

[Q09] 创建唯一索引
来源：http://qra.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rtf.gogol.net.cn

[Q10] 插入单行
来源：http://qli.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kif.zhoulong.xyz

[Q11] 一次插入多行
来源：http://luo.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yps.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://dnp.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://old.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xzs.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://sbq.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gir.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://wmh.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ltf.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fwk.xylfe.cn

[Q15] 查询全部
来源：http://hsx.zdqjudy.top

SELECT * FROM users;
来源：http://hbx.jqgfzy.top

[Q16] 查询指定列
来源：http://ftn.wangdashe.top

SELECT id, name FROM users;
来源：http://khk.yuanzhike.top

[Q17] 条件查询
来源：http://dat.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qzq.ehwqpu.com

[Q18] 模糊匹配
来源：http://vrk.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://smt.xuanzx.com

[Q19] 范围查询
来源：http://rxn.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pst.uphjek.com

[Q20] IN 列表
来源：http://ppx.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jpz.ehwqpu.com

[Q21] 空值判断
来源：http://oim.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vra.smart0.xyz

[Q22] 排序
来源：http://szv.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kkv.kuanghao11.cn

[Q23] 分页
来源：http://rms.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://srb.yj202588.top

[Q24] 去重
来源：http://bfe.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://svr.hywenlv.cn

[Q25] 只取前 N 条
来源：http://jma.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://opl.cqqwz.cn

[Q26] 计数
来源：http://kpw.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://cdc.9152youxi.cn

[Q27] 条件计数
来源：http://xae.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wpw.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://bug.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lcl.cheryme.top

[Q29] 最大最小值
来源：http://wox.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bea.daria6918.cn

[Q30] 分组统计
来源：http://qsl.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nzm.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://vmo.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xon.xinyue.icu

[Q32] 分组拼接字符串
来源：http://pvm.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xlu.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ckw.yuanzhike.top

[Q33] 多列分组
来源：http://olp.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hat.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://sek.9152youxi.cn

SELECT * FROM (
来源：http://ubp.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hkg.redwolf501.top

) t WHERE rn = 1;
来源：http://xjl.aibaodan.cn

[Q35] 内连接
来源：http://cfs.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ocy.hnqzz.top

[Q36] 左连接
来源：http://dvh.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qoa.zhaomingkeji.xyz

[Q37] 右连接
来源：http://tpm.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aij.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://lru.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fmy.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://otr.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jzb.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hvm.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hsa.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wnp.jinqigfzy.top

[Q41] 多表连接
来源：http://por.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fon.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://hwq.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://wgk.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://lii.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://mmc.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rst.hcnkem.com

[Q43] 标量子查询
来源：http://vpo.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://whn.wangdashe.top

[Q44] IN 子查询
来源：http://fde.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wdh.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://cna.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyx.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tvm.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mzp.sjlbkw.cn

[Q47] 与平均值比较
来源：http://jwo.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iwu.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://rgj.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jgg.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://bsn.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://mip.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://btn.yj20258888.top

[Q50] 批量更新
来源：http://jyh.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qgx.jinqigfzy.top

[Q51] 用子查询更新
来源：http://yeo.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://umc.gogol.net.cn

[Q52] 删除指定行
来源：http://hvf.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://oqc.nanxuanxn.top

[Q53] 按条件删除
来源：http://sqx.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ilz.quarkkingdee.top

[Q54] 清空表
来源：http://pld.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://wwa.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://zjh.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sat.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://xly.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tjf.fktsv.cn

[Q57] 行号
来源：http://fks.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://egw.quarkkingdee.top

[Q58] 累计求和
来源：http://jyi.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iwj.316326.xyz

[Q59] 分组内累计
来源：http://ybh.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vcr.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://vrl.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://msk.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oak.pycfn.com

[Q61] 移动平均
来源：http://ewa.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gal.yangfankeji.com

[Q62] 分组占比
来源：http://evy.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nrj.tanke756.top

[Q63] 开启事务
来源：http://fbl.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jay.hywenlv.cn

[Q64] 提交事务
来源：http://cel.hesvh.cn

COMMIT;
来源：http://oan.sjlbkw.cn

[Q65] 回滚事务
来源：http://ilp.nwbrower.top

ROLLBACK;
来源：http://mqu.yangfankeji.com

[Q66] 行锁查询
来源：http://bmy.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rgg.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://mfi.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdb.havefunace.top

[Q68] 保存点
来源：http://avy.aibaodan.cn

SAVEPOINT sp1;
来源：http://hxs.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://htz.9152youxi.cn

[Q69] 查看执行计划
来源：http://fzf.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://apm.52xcode.cn

[Q70] 更新统计信息
来源：http://wmv.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://jhz.hywenlv.cn

[Q71] 查看建表语句
来源：http://whf.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ekc.hysaishi.cn

[Q72] 查看索引
来源：http://opk.sysykeji.top

SHOW INDEX FROM users;
来源：http://hpo.svipenyu.cn

[Q73] 查看表状态
来源：http://zmn.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://saf.cucudq.cn

[Q74] 强制使用索引
来源：http://zcb.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mrn.uphjek.com

[Q75] 日期格式化
来源：http://knb.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tjw.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ged.cdnleiting.top

[Q76] 按天统计
来源：http://rtg.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dgs.shuidangran.top

[Q77] 时间加减
来源：http://tae.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://czf.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://rdk.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ety.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://hac.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ghf.yongpay.top

[Q80] 字符串截取
来源：http://xvy.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://khf.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://svc.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cbz.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://dsq.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zic.hammf.cn

[Q83] 大小写转换
来源：http://pci.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fal.yj202588.top

[Q84] 去除首尾空格
来源：http://ufl.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://ups.svipenyu.cn

[Q85] 数值取整
来源：http://nkr.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bkr.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://iuh.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kmz.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://iml.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uun.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://mco.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jre.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://llh.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://klw.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bae.shuidangran.top

[Q90] 生成序号列
来源：http://hrw.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nkk.sysykeji.top

================================================================================
来源：http://lmj.cucudq.cn

R. Bash 专题
来源：http://qbc.yangfankeji.com

================================================================================
来源：http://cqm.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://swn.yj202588.top

#!/usr/bin/env bash
来源：http://ffn.yongpay.top

set -euo pipefail
来源：http://jqn.sweek.top

[R02] 变量赋值与使用
来源：http://lcm.fzhhl.top

name="Tom"; echo "$name"
来源：http://bgc.hnxiangtu.top

[R03] 只读变量
来源：http://rrm.ehwqpu.com

readonly PI=3.14
来源：http://aan.dianchejie.cn

[R04] 位置参数
来源：http://opt.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hiz.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://jbu.tarul.cn

name="${1:-default}"
来源：http://uxy.yangfankeji.com

[R06] 判断命令是否存在
来源：http://zhv.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmt.nanxuanxn.top

[R07] if 判断文件
来源：http://exb.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jqh.sysykeji.top

[R08] 数值比较
来源：http://brq.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wef.daxiang520.top

[R09] 字符串比较
来源：http://kxq.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zkn.bbcook.cn

[R10] 正则匹配
来源：http://awx.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kuy.shanyushiyangkeji.top

[R11] case 多分支
来源：http://tng.shanyushiyangtech.top

case "$1" in
来源：http://fvf.xuetiantiany.cn

start) echo "启动" ;;
来源：http://yfb.nwbrower.top

stop)  echo "停止" ;;
来源：http://dif.hammf.cn

*)     echo "未知命令" ;;
来源：http://tvy.shuidangran.top

esac
来源：http://jrp.shangyingyoupin.top

[R12] for 遍历文件
来源：http://ytu.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://czp.hammf.cn

[R13] for 计数循环
来源：http://mqm.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://mwz.wangshuangyany.cn

[R14] C 风格 for
来源：http://zvy.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://imo.andypj.xyz

[R15] while 逐行读文件
来源：http://jph.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kaj.zhiwuduotai.top

[R16] until 等待条件
来源：http://tig.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wmj.fehbvm.com

[R17] 数组定义与取值
来源：http://qdh.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://lhe.cheryme.top

[R18] 遍历数组
来源：http://bwp.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqk.yongpay.top

[R19] 数组长度
来源：http://vat.jyoumei.cn

echo "${#arr[@]}"
来源：http://dtm.haohaochexian.top

[R20] 关联数组（字典）
来源：http://nxv.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qww.xuetiantiany.cn

[R21] 字符串长度
来源：http://isd.guannengcc.top

echo "${#s}"
来源：http://vdp.xuanzx.com

[R22] 截取子串
来源：http://mil.guowangkeji.top

echo "${s:0:5}"
来源：http://csu.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://zxv.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xxl.bjfxy.top

[R24] 大小写转换
来源：http://wam.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://lom.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://krj.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yre.52xcode.cn

[R26] 命令替换
来源：http://npx.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://xkr.jinqigufen.top

[R27] 算术展开
来源：http://tpn.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://whe.0kj1m.cn

[R28] 浮点运算
来源：http://oyv.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://rjz.xziqi.cn

[R29] 定义函数
来源：http://hdk.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yqg.zhijiandao.cn

[R30] 函数返回状态码
来源：http://ojx.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://imp.tianlin.xyz

[R31] 局部变量
来源：http://hrk.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://kak.zhijiandao.cn

[R32] 参数个数校验
来源：http://zvq.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yul.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://mba.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmr.yangfankeji.com

[R34] 退出时清理
来源：http://bnp.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://sbs.tianlin.xyz

[R35] 后台执行并等待
来源：http://yav.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://klk.iojbl.cn

[R36] 并发执行多个任务
来源：http://xgg.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dba.shuidangran.top

[R37] 把输出赋给变量
来源：http://vzf.zhoulong.xyz

files=$(ls -1)
来源：http://mdb.zhijiandao.cn

[R38] 管道串联
来源：http://lpg.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://imf.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://nxn.cashguo.top

cmd > out.log 2>&1
来源：http://xip.hesvh.cn

[R40] 追加写日志
来源：http://bvz.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://ddx.xziqi.cn

[R41] 丢弃输出
来源：http://odp.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://dze.sxryk.cn

[R42] 输入重定向
来源：http://auw.cashguo.top

wc -l < a.txt
来源：http://pqe.cucudq.cn

[R43] 按名字查找文件
来源：http://mnb.nwbrower.top

find . -name "*.log" -type f
来源：http://wyl.guannengcc.top

[R44] 按修改时间查找
来源：http://oja.52xcode.cn

find . -mtime -7 -type f
来源：http://gqc.daria6918.cn

[R45] 批量删除
来源：http://ziu.hnqzz.top

find . -name "*.tmp" -delete
来源：http://bmh.tanke756.top

[R46] 递归替换文件内容
来源：http://obh.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ofy.hongshengwenyu.top

[R47] sed 单行替换
来源：http://eei.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://eda.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://muw.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://hnv.yueranfly.top

[R49] awk 带条件
来源：http://sau.xinyue.icu


<!-- 参考信息 -->