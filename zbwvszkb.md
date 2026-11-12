代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://plx.jyoumei.cn

);
来源：http://aio.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://ymf.gotoacloud.top

CREATE TABLE orders (
来源：http://dce.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://moe.c1oappe.top

user_id INT NOT NULL,
来源：http://sso.xuanzx.com

amount DECIMAL(10, 2),
来源：http://ssq.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hkl.yanxiufei.cn

);
来源：http://etk.uphjek.com

[Q03] 增加列
来源：http://qst.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvb.daxiang520.top

[Q04] 修改列类型
来源：http://bio.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qqi.redwolf501.top

[Q05] 重命名列
来源：http://rhr.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vgx.cdnleiting.top

[Q06] 删除列
来源：http://bva.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hcr.yj20258888.top

[Q07] 删除表
来源：http://cof.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://jif.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://qfu.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dsg.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://sms.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cws.xylfe.cn

[Q10] 插入单行
来源：http://mkk.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xgk.vehdjk.com

[Q11] 一次插入多行
来源：http://udj.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbu.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://cuu.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nqa.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vyo.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://irx.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vbv.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://drx.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zvc.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zgz.shzxlz.cn

[Q15] 查询全部
来源：http://enf.svipenyu.cn

SELECT * FROM users;
来源：http://rqg.yfazqb.com

[Q16] 查询指定列
来源：http://rut.aizwys.cn

SELECT id, name FROM users;
来源：http://jyt.shzxlz.cn

[Q17] 条件查询
来源：http://wnc.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhi.fktsv.cn

[Q18] 模糊匹配
来源：http://ezo.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ugf.chenjidiqi.icu

[Q19] 范围查询
来源：http://btl.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jei.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://dgj.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dom.zdbjq.cn

[Q21] 空值判断
来源：http://apt.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hje.yj20258.top

[Q22] 排序
来源：http://gdn.yuxming.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://smp.gaohongyu789.top

[Q23] 分页
来源：http://kfq.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kbs.fktsv.cn

[Q24] 去重
来源：http://rcx.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://pgc.sufxvd.cn

[Q25] 只取前 N 条
来源：http://njr.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://evw.ivvv.top

[Q26] 计数
来源：http://jbv.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://lzr.yueranfly.top

[Q27] 条件计数
来源：http://oxf.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jle.svipenyu.cn

[Q28] 求和与平均
来源：http://tjf.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://okm.0kj1m.cn

[Q29] 最大最小值
来源：http://azz.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgd.daria6918.cn

[Q30] 分组统计
来源：http://sat.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ubq.pycfn.com

[Q31] 分组后过滤
来源：http://qvg.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zbm.316326.xyz

[Q32] 分组拼接字符串
来源：http://isn.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lxt.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyc.chenzaomai.com

[Q33] 多列分组
来源：http://prs.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mwa.gogol.net.cn

[Q34] 每组取第一条
来源：http://rna.fehbvm.com

SELECT * FROM (
来源：http://omh.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bzf.ctjpmb.com

) t WHERE rn = 1;
来源：http://nqb.zdbjq.cn

[Q35] 内连接
来源：http://lee.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hpv.tarul.cn

[Q36] 左连接
来源：http://ikn.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://asc.shanyushiyangtech.top

[Q37] 右连接
来源：http://efp.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rfn.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://zaa.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jal.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://vks.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cgn.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nhu.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://jzm.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rji.yvedp.cn

[Q41] 多表连接
来源：http://oig.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nue.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://ixw.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://phd.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://blm.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://uhv.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://htv.ybcxt.top

[Q43] 标量子查询
来源：http://fzy.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vau.smart0.xyz

[Q44] IN 子查询
来源：http://shk.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jjn.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://uxd.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akh.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tte.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nwd.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://eqp.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ioe.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://rjl.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ivo.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://bdp.sufxvd.cn

[Q49] 更新单行
来源：http://uqw.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xpr.xuanzx.com

[Q50] 批量更新
来源：http://wdc.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yfa.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://qaw.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sbc.yangfankeji.com

[Q52] 删除指定行
来源：http://qye.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://eiv.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://umx.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://txt.fehbvm.com

[Q54] 清空表
来源：http://hlb.hcnkem.com

TRUNCATE TABLE logs;
来源：http://lzp.fktsv.cn

[Q55] 排名（并列占位）
来源：http://ihs.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://erd.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://jjd.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://weh.tarul.cn

[Q57] 行号
来源：http://xfj.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jdu.kuanghao11.cn

[Q58] 累计求和
来源：http://vrc.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfz.fengsongda.top

[Q59] 分组内累计
来源：http://zvt.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://smy.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://qbi.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://emq.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qpy.nwbrower.top

[Q61] 移动平均
来源：http://vdf.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wnv.316326.xyz

[Q62] 分组占比
来源：http://zog.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nqt.jqgufenzy.top

[Q63] 开启事务
来源：http://htv.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tdv.yj20258.top

[Q64] 提交事务
来源：http://yqo.hongshengwenyu.top

COMMIT;
来源：http://lbm.yj20258.top

[Q65] 回滚事务
来源：http://hbh.iojbl.cn

ROLLBACK;
来源：http://ivp.sweek.top

[Q66] 行锁查询
来源：http://tcc.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yjy.9152youxi.cn

[Q67] 设置隔离级别
来源：http://wcw.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ayq.shanyushiyangkeji.top

[Q68] 保存点
来源：http://hzp.havefunace.top

SAVEPOINT sp1;
来源：http://xxz.shuidangran.top

ROLLBACK TO sp1;
来源：http://zsp.jinqigfzy.top

[Q69] 查看执行计划
来源：http://qaq.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://slk.epnwcf.com

[Q70] 更新统计信息
来源：http://ubf.fengsongda.top

ANALYZE TABLE users;
来源：http://fwh.hnqzz.top

[Q71] 查看建表语句
来源：http://dih.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uvg.jlsjyb.cn

[Q72] 查看索引
来源：http://jdf.cucudq.cn

SHOW INDEX FROM users;
来源：http://bgp.sysykeji.top

[Q73] 查看表状态
来源：http://esl.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://drr.guannengcc.top

[Q74] 强制使用索引
来源：http://dxl.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rrp.daria6918.cn

[Q75] 日期格式化
来源：http://ccw.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xlf.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jjg.feifeiyinyue.top

[Q76] 按天统计
来源：http://hlq.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dje.gotoacloud.top

[Q77] 时间加减
来源：http://sui.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whr.yongpay.top

[Q78] 当前时间
来源：http://lml.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mlj.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://udw.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tcz.vqdsnc.cn

[Q80] 字符串截取
来源：http://blc.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bvi.daria6918.cn

[Q81] 字符串替换
来源：http://pya.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cmm.yj20258.top

[Q82] 字符长度与字节长度
来源：http://jna.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qgf.hammf.cn

[Q83] 大小写转换
来源：http://vet.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uwl.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://kwf.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://imm.cashguo.top

[Q85] 数值取整
来源：http://jpd.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rza.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://gpp.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pgo.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://kfg.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://itm.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://ctl.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ftz.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jrj.xuanzx.com

[Q89] 判断表是否存在
来源：http://yoa.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uey.xylfe.cn

[Q90] 生成序号列
来源：http://xmc.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pzr.zhiwuduotai.top

================================================================================
来源：http://xfm.dianchejie.cn

R. Bash 专题
来源：http://qod.andypj.xyz

================================================================================
来源：http://odm.yj20258888.top

[R01] shebang 与严格模式
来源：http://uvt.hysaishi.cn

#!/usr/bin/env bash
来源：http://abo.vqdsnc.cn

set -euo pipefail
来源：http://ytr.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://rtd.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://hux.havefunace.top

[R03] 只读变量
来源：http://byr.fengsongda.top

readonly PI=3.14
来源：http://ulc.chenjidiqi.icu

[R04] 位置参数
来源：http://btc.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bln.bjfxy.top

[R05] 参数默认值
来源：http://hmm.tanke756.top

name="${1:-default}"
来源：http://uoc.zycfv.cn

[R06] 判断命令是否存在
来源：http://jnx.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dcn.redwolf501.top

[R07] if 判断文件
来源：http://uph.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxn.sjlbkw.cn

[R08] 数值比较
来源：http://avz.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gvw.uphjek.com

[R09] 字符串比较
来源：http://khe.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xkk.jlsjyb.cn

[R10] 正则匹配
来源：http://wiw.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aej.sxryk.cn

[R11] case 多分支
来源：http://ozj.cashguo.top

case "$1" in
来源：http://jbc.guowangkeji.top

start) echo "启动" ;;
来源：http://vau.gotoacloud.top

stop)  echo "停止" ;;
来源：http://hxs.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://dsr.316326.xyz

esac
来源：http://tcr.gzhubu.top

[R12] for 遍历文件
来源：http://ouw.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://plw.epnwcf.com

[R13] for 计数循环
来源：http://hdp.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://lkj.meibo888.top

[R14] C 风格 for
来源：http://mdr.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nst.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://iha.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dsg.sysykeji.top

[R16] until 等待条件
来源：http://sle.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bui.tanke756.top

[R17] 数组定义与取值
来源：http://ust.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://yst.316326.xyz

[R18] 遍历数组
来源：http://saz.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lkb.xuetiantiany.cn

[R19] 数组长度
来源：http://qqv.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://egr.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://jjb.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rys.uphjek.com

[R21] 字符串长度
来源：http://qox.jqgufenzy.top

echo "${#s}"
来源：http://xjn.c1oappe.top

[R22] 截取子串
来源：http://qss.9152youxi.cn

echo "${s:0:5}"
来源：http://glw.shangyingyoupin.top

[R23] 字符串替换
来源：http://tph.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qhy.tian-w.cn

[R24] 大小写转换
来源：http://zlx.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://sns.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://psm.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pin.tianlin.xyz

[R26] 命令替换
来源：http://oec.havefunace.top

now=$(date +%F); echo "$now"
来源：http://rfj.hcnkem.com

[R27] 算术展开
来源：http://axv.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://mix.xuetiantiany.cn

[R28] 浮点运算
来源：http://hpe.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://pus.hfpthk.cn

[R29] 定义函数
来源：http://zst.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vay.hnxiangtu.top

[R30] 函数返回状态码
来源：http://frb.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://wsc.fktsv.cn

[R31] 局部变量
来源：http://vvw.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://axb.daxiang520.top

[R32] 参数个数校验
来源：http://rkd.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zog.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://mfp.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eox.zhijiandao.cn

[R34] 退出时清理
来源：http://svz.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://jiw.hywenlv.cn

[R35] 后台执行并等待
来源：http://pms.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kcs.aibaodan.cn

[R36] 并发执行多个任务
来源：http://ebq.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://phx.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://aza.jyoumei.cn

files=$(ls -1)
来源：http://edu.zhongyouzk.top

[R38] 管道串联
来源：http://ieq.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://iea.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://qmh.fengsongda.top

cmd > out.log 2>&1
来源：http://bmw.hnxiangtu.top

[R40] 追加写日志
来源：http://axz.bbcook.cn

echo "log" >> out.log
来源：http://yzf.vqdsnc.cn

[R41] 丢弃输出
来源：http://mus.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://vyl.yj20258.top

[R42] 输入重定向
来源：http://eir.zhengqikj.top

wc -l < a.txt
来源：http://nrw.kuanghao11.cn

[R43] 按名字查找文件
来源：http://lwj.jyoumei.cn

find . -name "*.log" -type f
来源：http://bmp.cashguo.top

[R44] 按修改时间查找
来源：http://gdd.hesvh.cn

find . -mtime -7 -type f
来源：http://kfn.jinqigufen.top

[R45] 批量删除
来源：http://sfv.yuxming.cn

find . -name "*.tmp" -delete
来源：http://lan.svipenyu.cn

[R46] 递归替换文件内容
来源：http://tav.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lug.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://wcq.meibo888.top


<!-- 参考信息 -->