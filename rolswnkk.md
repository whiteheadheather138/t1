代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ack.ctjpmb.com

);
来源：http://xsu.pycfn.com

[Q02] 创建带外键的表
来源：http://zqi.fzhhl.top

CREATE TABLE orders (
来源：http://rii.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jux.vqdsnc.cn

user_id INT NOT NULL,
来源：http://mfe.nwbrower.top

amount DECIMAL(10, 2),
来源：http://vcx.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gnl.pycfn.com

);
来源：http://ztd.jinqigfzy.top

[Q03] 增加列
来源：http://tqw.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://thu.yangfankeji.com

[Q04] 修改列类型
来源：http://ngj.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mma.fengsongda.top

[Q05] 重命名列
来源：http://ofh.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://llc.pycfn.com

[Q06] 删除列
来源：http://ufm.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://jsm.yongpay.top

[Q07] 删除表
来源：http://yoh.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://uta.yanxiufei.cn

[Q08] 创建普通索引
来源：http://osl.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ywa.bbcook.cn

[Q09] 创建唯一索引
来源：http://woj.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pkf.yfazqb.com

[Q10] 插入单行
来源：http://hrh.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iwv.zhengqikj.top

[Q11] 一次插入多行
来源：http://poz.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kai.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://cik.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://vcc.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxy.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://vtj.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lqz.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://wdz.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oue.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yac.xuanzx.com

[Q15] 查询全部
来源：http://emh.chenzaomai.com

SELECT * FROM users;
来源：http://xgc.yangfankeji.com

[Q16] 查询指定列
来源：http://wco.daria6918.cn

SELECT id, name FROM users;
来源：http://sfl.jinqigufen.top

[Q17] 条件查询
来源：http://est.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mwn.mhx1999.top

[Q18] 模糊匹配
来源：http://bso.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://evx.nanxuanxn.top

[Q19] 范围查询
来源：http://fjn.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vpl.tarul.cn

[Q20] IN 列表
来源：http://jlm.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pff.chenzaomai.com

[Q21] 空值判断
来源：http://xcm.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://awb.aizwys.cn

[Q22] 排序
来源：http://ncv.aibaodan.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eir.nanxinkj.top

[Q23] 分页
来源：http://smd.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ksz.nwbrower.top

[Q24] 去重
来源：http://ghc.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://bnj.iojbl.cn

[Q25] 只取前 N 条
来源：http://faf.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ejn.316326.xyz

[Q26] 计数
来源：http://bpm.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://yse.redwolf501.top

[Q27] 条件计数
来源：http://jfw.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qpr.ppjwa.cn

[Q28] 求和与平均
来源：http://qbz.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vuv.yuanzhike.top

[Q29] 最大最小值
来源：http://xzp.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zzz.wangdashe.top

[Q30] 分组统计
来源：http://awo.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://noo.ctjpmb.com

[Q31] 分组后过滤
来源：http://dfi.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qkj.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://ike.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lpc.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qmm.tianlin.xyz

[Q33] 多列分组
来源：http://bvf.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hbw.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://ihf.ywan-chungtsiang.top

SELECT * FROM (
来源：http://ceo.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mwv.zhongyouzk.top

) t WHERE rn = 1;
来源：http://imh.cqqwz.cn

[Q35] 内连接
来源：http://dpz.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqv.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://qkz.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fih.fengsongda.top

[Q37] 右连接
来源：http://jkp.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xti.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://yqp.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ido.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://lxg.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bod.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jxy.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hxz.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jth.guannengcc.top

[Q41] 多表连接
来源：http://nkn.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tme.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://jxv.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://imj.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://lqd.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://tqx.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://njk.jlsjyb.cn

[Q43] 标量子查询
来源：http://ztx.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rbe.sweek.top

[Q44] IN 子查询
来源：http://fdt.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ijj.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://wyi.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjl.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://lji.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aut.mhx1999.top

[Q47] 与平均值比较
来源：http://kqw.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ezv.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://sxg.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kli.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://lad.chenlongwang.top

[Q49] 更新单行
来源：http://ihg.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://etq.wangshuangyany.cn

[Q50] 批量更新
来源：http://wdc.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wco.fktsv.cn

[Q51] 用子查询更新
来源：http://apy.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hex.chenzaomai.com

[Q52] 删除指定行
来源：http://dyp.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://fnq.tianlin.xyz

[Q53] 按条件删除
来源：http://qqs.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://poa.jinqigufen.top

[Q54] 清空表
来源：http://qck.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://jrd.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://ivc.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://txc.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://coe.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dtn.yangfankeji.com

[Q57] 行号
来源：http://pxa.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oqf.zhengqikj.top

[Q58] 累计求和
来源：http://tre.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rfn.ppjwa.cn

[Q59] 分组内累计
来源：http://pnl.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zme.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://wsz.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vrs.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://njw.jqgfzy.top

[Q61] 移动平均
来源：http://xxw.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://erh.kuanghao11.cn

[Q62] 分组占比
来源：http://zxh.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mzn.ctjpmb.com

[Q63] 开启事务
来源：http://xav.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xim.zdbjq.cn

[Q64] 提交事务
来源：http://cyb.tarul.cn

COMMIT;
来源：http://xrm.gzhubu.top

[Q65] 回滚事务
来源：http://ldz.nanxinkj.top

ROLLBACK;
来源：http://ajv.nwbrower.top

[Q66] 行锁查询
来源：http://vcc.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bkr.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://ube.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hiv.yongpay.top

[Q68] 保存点
来源：http://yul.c1oappe.top

SAVEPOINT sp1;
来源：http://dvy.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://kwb.chenzaomai.com

[Q69] 查看执行计划
来源：http://mbd.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zuz.wangdashe.top

[Q70] 更新统计信息
来源：http://wku.ivvv.top

ANALYZE TABLE users;
来源：http://nhi.jiagoushi.top

[Q71] 查看建表语句
来源：http://ovo.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lrl.yongpay.top

[Q72] 查看索引
来源：http://jsq.cucudq.cn

SHOW INDEX FROM users;
来源：http://usf.iojbl.cn

[Q73] 查看表状态
来源：http://bnf.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ikd.yanxiufei.cn

[Q74] 强制使用索引
来源：http://yyv.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jtv.bjfxy.top

[Q75] 日期格式化
来源：http://mbk.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwp.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cau.cashguo.top

[Q76] 按天统计
来源：http://azm.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://itx.shanyushiyangtech.top

[Q77] 时间加减
来源：http://cmf.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ztm.zhongyouzk.top

[Q78] 当前时间
来源：http://bvh.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yju.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://olo.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iom.cheryme.top

[Q80] 字符串截取
来源：http://upj.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bqx.xziqi.cn

[Q81] 字符串替换
来源：http://gbm.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lop.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://tkb.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xnd.dashuyun.cn

[Q83] 大小写转换
来源：http://atf.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://see.zycfv.cn

[Q84] 去除首尾空格
来源：http://koo.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://aro.hfpthk.cn

[Q85] 数值取整
来源：http://xcb.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cew.yj20258.top

[Q86] 读取 JSON 字段
来源：http://mpm.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ezl.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://sed.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://epl.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://neg.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ndo.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lul.fktsv.cn

[Q89] 判断表是否存在
来源：http://frs.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hra.xuetiantiany.cn

[Q90] 生成序号列
来源：http://emf.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vjs.dianchejie.cn

================================================================================
来源：http://kla.epnwcf.com

R. Bash 专题
来源：http://waa.shanyushiyangtech.top

================================================================================
来源：http://wlf.nanxinkj.top

[R01] shebang 与严格模式
来源：http://bci.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://klo.shuidangran.top

set -euo pipefail
来源：http://wpe.zdbjq.cn

[R02] 变量赋值与使用
来源：http://mab.hcnkem.com

name="Tom"; echo "$name"
来源：http://nzb.kuanghao11.cn

[R03] 只读变量
来源：http://fly.c1oappe.top

readonly PI=3.14
来源：http://mac.shanyushiyangtech.top

[R04] 位置参数
来源：http://cqo.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zep.ydjk.org.cn

[R05] 参数默认值
来源：http://wkq.guannengcc.top

name="${1:-default}"
来源：http://obb.zhixingplan.top

[R06] 判断命令是否存在
来源：http://hqu.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lhr.vehdjk.com

[R07] if 判断文件
来源：http://fdp.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mda.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://lxi.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hjk.fanxiaobao.xyz

[R09] 字符串比较
来源：http://eiu.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://irf.jinqigfzy.top

[R10] 正则匹配
来源：http://dwh.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krz.yanxiufei.cn

[R11] case 多分支
来源：http://xfy.zhijiandao.cn

case "$1" in
来源：http://oxx.cdnleiting.top

start) echo "启动" ;;
来源：http://oqc.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://oys.aizwys.cn

*)     echo "未知命令" ;;
来源：http://jpw.jinqigfzy.top

esac
来源：http://bqw.haohaochexian.top

[R12] for 遍历文件
来源：http://enq.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://jjm.yj202588.top

[R13] for 计数循环
来源：http://vty.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://kcw.pengpengdd.cyou

[R14] C 风格 for
来源：http://gtg.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vjg.hammf.cn

[R15] while 逐行读文件
来源：http://rlo.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qal.316326.xyz

[R16] until 等待条件
来源：http://jdj.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwp.xziqi.cn

[R17] 数组定义与取值
来源：http://nys.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mhx.ctjpmb.com

[R18] 遍历数组
来源：http://pun.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cax.316326.xyz

[R19] 数组长度
来源：http://fwj.yanxiufei.cn

echo "${#arr[@]}"
来源：http://upg.bbcook.cn

[R20] 关联数组（字典）
来源：http://mff.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zkq.zhijiandao.cn

[R21] 字符串长度
来源：http://pxz.hesvh.cn

echo "${#s}"
来源：http://sqn.hnxiangtu.top

[R22] 截取子串
来源：http://sef.xuetiantiany.cn

echo "${s:0:5}"
来源：http://vfz.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://gcf.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qzh.jianghu66.top

[R24] 大小写转换
来源：http://kbg.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://luy.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://cjx.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kzv.fktsv.cn

[R26] 命令替换
来源：http://zvk.tanke756.top

now=$(date +%F); echo "$now"
来源：http://ufz.chenjidiqi.icu

[R27] 算术展开
来源：http://ohl.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://hfx.jyoumei.cn

[R28] 浮点运算
来源：http://vgf.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://tjm.kuanghao11.cn

[R29] 定义函数
来源：http://nef.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pzu.shuidangran.top

[R30] 函数返回状态码
来源：http://iop.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://tir.yj20258.top

[R31] 局部变量
来源：http://tyu.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://uze.tianlin.xyz

[R32] 参数个数校验
来源：http://bau.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mef.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://lsp.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eft.vqdsnc.cn

[R34] 退出时清理
来源：http://tjc.bjfxy.top

trap 'rm -f "$tmp"' EXIT
来源：http://gyj.zhixingplan.top

[R35] 后台执行并等待
来源：http://izq.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jlv.epnwcf.com

[R36] 并发执行多个任务
来源：http://jzx.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhp.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://soq.fktsv.cn

files=$(ls -1)
来源：http://xhc.meibo888.top

[R38] 管道串联
来源：http://hyt.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://eba.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://usx.zdqjudy.top

cmd > out.log 2>&1
来源：http://ypy.hnxiangtu.top

[R40] 追加写日志
来源：http://tem.meibo888.top

echo "log" >> out.log
来源：http://bzg.vqdsnc.cn

[R41] 丢弃输出
来源：http://frt.zycfv.cn

cmd >/dev/null 2>&1
来源：http://pbl.wangdashe.top

[R42] 输入重定向
来源：http://icq.0kj1m.cn

wc -l < a.txt
来源：http://kqg.ppjwa.cn

[R43] 按名字查找文件
来源：http://fft.sxryk.cn

find . -name "*.log" -type f
来源：http://mzk.gzhubu.top

[R44] 按修改时间查找
来源：http://sop.yj20258.top

find . -mtime -7 -type f
来源：http://rxu.xylfe.cn

[R45] 批量删除
来源：http://tqv.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://mpp.jinqigufen.top

[R46] 递归替换文件内容
来源：http://jes.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://djm.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://xjs.9152youxi.cn


<!-- 参考信息 -->