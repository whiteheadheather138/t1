代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://axw.fengsongda.top

);
来源：http://sdx.gogol.net.cn

[Q02] 创建带外键的表
来源：http://daq.yfazqb.com

CREATE TABLE orders (
来源：http://vsv.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uib.ydzc1.top

user_id INT NOT NULL,
来源：http://xgu.tanke756.top

amount DECIMAL(10, 2),
来源：http://crz.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aog.wangdashe.top

);
来源：http://iex.chenlongwang.top

[Q03] 增加列
来源：http://iuv.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://izr.gogol.net.cn

[Q04] 修改列类型
来源：http://dsf.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vuk.xziqi.cn

[Q05] 重命名列
来源：http://krj.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hqw.sjlbkw.cn

[Q06] 删除列
来源：http://rxu.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://dgn.bbcook.cn

[Q07] 删除表
来源：http://cay.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://iao.gzhubu.top

[Q08] 创建普通索引
来源：http://ljr.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mcd.svipenyu.cn

[Q09] 创建唯一索引
来源：http://ojm.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jxs.fehbvm.com

[Q10] 插入单行
来源：http://ntu.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://atk.redwolf501.top

[Q11] 一次插入多行
来源：http://wes.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cww.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://ufa.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://tjf.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://agh.hysaishi.cn

[Q13] 忽略重复插入
来源：http://ejg.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rsk.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://zbu.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ywf.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ggl.fzhhl.top

[Q15] 查询全部
来源：http://pgb.nwbrower.top

SELECT * FROM users;
来源：http://oic.316326.xyz

[Q16] 查询指定列
来源：http://ind.yj202588.top

SELECT id, name FROM users;
来源：http://pfz.ppjwa.cn

[Q17] 条件查询
来源：http://mdv.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xaq.kuanghao11.cn

[Q18] 模糊匹配
来源：http://fdw.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dzp.daxiang520.top

[Q19] 范围查询
来源：http://obq.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uey.redwolf501.top

[Q20] IN 列表
来源：http://cvm.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://evm.iojbl.cn

[Q21] 空值判断
来源：http://leq.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jsl.hcnkem.com

[Q22] 排序
来源：http://xvh.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zrl.dashuyun.cn

[Q23] 分页
来源：http://jjw.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dom.ydzc1.top

[Q24] 去重
来源：http://avz.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://ifa.vehdjk.com

[Q25] 只取前 N 条
来源：http://apy.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vmv.cashguo.top

[Q26] 计数
来源：http://yos.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://rks.cucudq.cn

[Q27] 条件计数
来源：http://dpr.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jjf.xziqi.cn

[Q28] 求和与平均
来源：http://qay.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://khw.cdnleiting.top

[Q29] 最大最小值
来源：http://zeh.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dua.jyoumei.cn

[Q30] 分组统计
来源：http://chr.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://llz.pycfn.com

[Q31] 分组后过滤
来源：http://aah.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://frn.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://nsl.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://got.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cov.zycfv.cn

[Q33] 多列分组
来源：http://yul.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bgr.daria6918.cn

[Q34] 每组取第一条
来源：http://lsq.haohaochexian.top

SELECT * FROM (
来源：http://inl.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yoi.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://rhp.wangshuangyany.cn

[Q35] 内连接
来源：http://sve.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bsm.hesvh.cn

[Q36] 左连接
来源：http://xeh.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kxh.shanyushiyangtech.top

[Q37] 右连接
来源：http://mmd.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvm.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://szk.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cnw.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://dyt.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cjw.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://djz.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qjv.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jwa.haohaochexian.top

[Q41] 多表连接
来源：http://qnq.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vbt.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://nsw.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://gqy.yj20258.top

[Q42] 连接条件附加过滤
来源：http://cpx.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://kbw.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bdi.pengpengdd.cyou

[Q43] 标量子查询
来源：http://yfb.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vll.jyoumei.cn

[Q44] IN 子查询
来源：http://jpb.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://suv.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://swx.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhb.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jdf.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgf.dashuyun.cn

[Q47] 与平均值比较
来源：http://jqn.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mzi.tanke756.top

[Q48] CTE 公用表表达式
来源：http://brl.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qox.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://lzv.guannengcc.top

[Q49] 更新单行
来源：http://bte.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ysw.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://jac.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lur.hnxiangtu.top

[Q51] 用子查询更新
来源：http://stu.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iyx.wangdashe.top

[Q52] 删除指定行
来源：http://nhs.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://erp.nwbrower.top

[Q53] 按条件删除
来源：http://mya.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sed.daria6918.cn

[Q54] 清空表
来源：http://yer.havefunace.top

TRUNCATE TABLE logs;
来源：http://ukw.tanke756.top

[Q55] 排名（并列占位）
来源：http://uqx.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mye.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://vga.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dym.kuanghao11.cn

[Q57] 行号
来源：http://vxm.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yow.zhixingplan.top

[Q58] 累计求和
来源：http://msw.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://btr.zhengqikj.top

[Q59] 分组内累计
来源：http://wjh.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nlr.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://upa.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uoj.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jjn.chenjidiqi.icu

[Q61] 移动平均
来源：http://shq.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jjh.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://trf.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vwi.tarul.cn

[Q63] 开启事务
来源：http://nfi.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vup.shangyingyoupin.top

[Q64] 提交事务
来源：http://sxn.hesvh.cn

COMMIT;
来源：http://jdl.cdnleiting.top

[Q65] 回滚事务
来源：http://vcm.hfpthk.cn

ROLLBACK;
来源：http://zbj.yj20258.top

[Q66] 行锁查询
来源：http://gux.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pve.epnwcf.com

[Q67] 设置隔离级别
来源：http://obb.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://smb.ivvv.top

[Q68] 保存点
来源：http://zlk.cucudq.cn

SAVEPOINT sp1;
来源：http://vpa.tianlin.xyz

ROLLBACK TO sp1;
来源：http://hgc.snrcjt.cn

[Q69] 查看执行计划
来源：http://vle.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ylj.ppjwa.cn

[Q70] 更新统计信息
来源：http://fiu.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://ydj.yj202588.top

[Q71] 查看建表语句
来源：http://qyc.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ktm.fktsv.cn

[Q72] 查看索引
来源：http://oox.redwolf501.top

SHOW INDEX FROM users;
来源：http://toe.gogol.net.cn

[Q73] 查看表状态
来源：http://hqg.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://waz.jyoumei.cn

[Q74] 强制使用索引
来源：http://wxm.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://krf.hammf.cn

[Q75] 日期格式化
来源：http://lpq.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nzq.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ysi.tian-w.cn

[Q76] 按天统计
来源：http://zvc.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jyt.xuetiantiany.cn

[Q77] 时间加减
来源：http://mxa.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bpn.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://oeq.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kkr.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://jeu.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ihi.hesvh.cn

[Q80] 字符串截取
来源：http://dpm.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uya.epnwcf.com

[Q81] 字符串替换
来源：http://qok.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zde.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://smo.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://msx.andypj.xyz

[Q83] 大小写转换
来源：http://clk.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fmp.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://ajj.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://lwn.fengsongda.top

[Q85] 数值取整
来源：http://yyr.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://znb.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://nwj.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dhz.redwolf501.top

[Q87] JSON 字段做条件
来源：http://oem.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://brd.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://vvi.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qsj.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lqp.guannengcc.top

[Q89] 判断表是否存在
来源：http://tme.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aor.andypj.xyz

[Q90] 生成序号列
来源：http://kao.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dot.zhongyouzk.top

================================================================================
来源：http://zdz.jqgufenzy.top

R. Bash 专题
来源：http://mvl.jinqigufen.top

================================================================================
来源：http://zgo.gzhubu.top

[R01] shebang 与严格模式
来源：http://kdr.aibaodan.cn

#!/usr/bin/env bash
来源：http://fuq.tarul.cn

set -euo pipefail
来源：http://pcu.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://srq.9152youxi.cn

name="Tom"; echo "$name"
来源：http://ptp.xuanzx.com

[R03] 只读变量
来源：http://wfm.yfazqb.com

readonly PI=3.14
来源：http://dle.sufxvd.cn

[R04] 位置参数
来源：http://joj.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://teu.uphjek.com

[R05] 参数默认值
来源：http://ugs.zycfv.cn

name="${1:-default}"
来源：http://tyx.jiagoushi.top

[R06] 判断命令是否存在
来源：http://lbl.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zoa.cdnleiting.top

[R07] if 判断文件
来源：http://gzp.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xps.yanxiufei.cn

[R08] 数值比较
来源：http://cvw.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://opm.zdbjq.cn

[R09] 字符串比较
来源：http://lna.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dia.fanxiaobao.xyz

[R10] 正则匹配
来源：http://mdx.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mko.ydzc1.top

[R11] case 多分支
来源：http://qkv.jinqigufen.top

case "$1" in
来源：http://ttr.zhijiandao.cn

start) echo "启动" ;;
来源：http://xab.sysykeji.top

stop)  echo "停止" ;;
来源：http://uss.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://vdz.chenzaomai.com

esac
来源：http://zaq.zhongyouzk.top

[R12] for 遍历文件
来源：http://zxh.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://prs.hywenlv.cn

[R13] for 计数循环
来源：http://ypa.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nir.sysykeji.top

[R14] C 风格 for
来源：http://iad.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://evr.ppjwa.cn

[R15] while 逐行读文件
来源：http://mwi.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blm.jqgufenzy.top

[R16] until 等待条件
来源：http://nvh.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cjs.ivvv.top

[R17] 数组定义与取值
来源：http://mcs.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://ofq.guowangkeji.top

[R18] 遍历数组
来源：http://ydw.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xei.yj20258888.top

[R19] 数组长度
来源：http://cmt.9152youxi.cn

echo "${#arr[@]}"
来源：http://pvt.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://mqn.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zsl.316326.xyz

[R21] 字符串长度
来源：http://lmn.gogol.net.cn

echo "${#s}"
来源：http://afp.hysaishi.cn

[R22] 截取子串
来源：http://nwc.daxiang520.top

echo "${s:0:5}"
来源：http://npy.sxryk.cn

[R23] 字符串替换
来源：http://tlj.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://plb.feifeiyinyue.top

[R24] 大小写转换
来源：http://lzv.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xnx.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://lwu.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ume.shzxlz.cn

[R26] 命令替换
来源：http://abs.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://dkx.ivvv.top

[R27] 算术展开
来源：http://xrj.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://mgb.jinqigufen.top

[R28] 浮点运算
来源：http://rfo.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://rjt.vehdjk.com

[R29] 定义函数
来源：http://czn.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvb.nanxuanxn.top

[R30] 函数返回状态码
来源：http://mcy.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://cxa.nanxuanxn.top

[R31] 局部变量
来源：http://mdj.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://jpo.pengpengdd.cyou

[R32] 参数个数校验
来源：http://lxp.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tfw.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://sph.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nrp.fanxiaobao.xyz

[R34] 退出时清理
来源：http://ded.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://qcr.zhixingplan.top

[R35] 后台执行并等待
来源：http://tqo.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qzr.hnqzz.top

[R36] 并发执行多个任务
来源：http://zaf.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rzs.guannengcc.top

[R37] 把输出赋给变量
来源：http://vwr.quarkkingdee.top

files=$(ls -1)
来源：http://fst.chenzaomai.com

[R38] 管道串联
来源：http://ogw.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://tlp.birdmap.top

[R39] 重定向标准输出与错误
来源：http://wzp.xziqi.cn

cmd > out.log 2>&1
来源：http://yqw.yvedp.cn

[R40] 追加写日志
来源：http://yll.pycfn.com

echo "log" >> out.log
来源：http://lrs.ydzc1.top

[R41] 丢弃输出
来源：http://ful.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://dwl.nanxinkj.top

[R42] 输入重定向
来源：http://enj.yj202588.top

wc -l < a.txt
来源：http://yel.gogol.net.cn

[R43] 按名字查找文件
来源：http://zye.nanxinkj.top

find . -name "*.log" -type f
来源：http://fji.meibo888.top

[R44] 按修改时间查找
来源：http://hrj.yangfankeji.com

find . -mtime -7 -type f
来源：http://nlt.fktsv.cn

[R45] 批量删除
来源：http://ohs.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://eda.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://fxt.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qll.hongshengwenyu.top

[R47] sed 单行替换
来源：http://axl.hesvh.cn


<!-- 参考信息 -->