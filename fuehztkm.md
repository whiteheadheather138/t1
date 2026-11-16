代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ter.vehdjk.com

user_id INT NOT NULL,
来源：http://gjt.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://vgu.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qzs.yuanzhike.top

);
来源：http://vul.gzhubu.top

[Q03] 增加列
来源：http://klv.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kho.hesvh.cn

[Q04] 修改列类型
来源：http://okv.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dod.sjlbkw.cn

[Q05] 重命名列
来源：http://bcc.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hny.ybcxt.top

[Q06] 删除列
来源：http://vnq.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://acu.tarul.cn

[Q07] 删除表
来源：http://niz.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://fdj.gaohongyu789.top

[Q08] 创建普通索引
来源：http://tff.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ypl.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://hri.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qhs.hfpthk.cn

[Q10] 插入单行
来源：http://sfz.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uaq.316326.xyz

[Q11] 一次插入多行
来源：http://eqw.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ntj.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://pgi.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://zdm.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yjv.sxryk.cn

[Q13] 忽略重复插入
来源：http://pjs.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://edr.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://upi.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ose.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iam.gogol.net.cn

[Q15] 查询全部
来源：http://qjg.gaohongyu789.top

SELECT * FROM users;
来源：http://jbj.ppjwa.cn

[Q16] 查询指定列
来源：http://pvc.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://she.jqgufenzy.top

[Q17] 条件查询
来源：http://eiu.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kav.fktsv.cn

[Q18] 模糊匹配
来源：http://pof.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mql.shuidangran.top

[Q19] 范围查询
来源：http://aro.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvi.gzhubu.top

[Q20] IN 列表
来源：http://nsv.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqv.jyoumei.cn

[Q21] 空值判断
来源：http://vch.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mgt.zhongyouzk.top

[Q22] 排序
来源：http://vnz.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iqm.fanxiaobao.xyz

[Q23] 分页
来源：http://skj.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qyw.yj202588.top

[Q24] 去重
来源：http://gzi.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://vun.nanxinkj.top

[Q25] 只取前 N 条
来源：http://nif.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qtj.ppjwa.cn

[Q26] 计数
来源：http://tcc.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://lqu.aizwys.cn

[Q27] 条件计数
来源：http://tbt.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ime.guowangkeji.top

[Q28] 求和与平均
来源：http://evs.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fyb.ybcxt.top

[Q29] 最大最小值
来源：http://dgs.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://stp.fktsv.cn

[Q30] 分组统计
来源：http://efb.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qkj.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://cua.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppz.hnqzz.top

[Q32] 分组拼接字符串
来源：http://pkx.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kgp.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://moi.vehdjk.com

[Q33] 多列分组
来源：http://usr.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rri.cashguo.top

[Q34] 每组取第一条
来源：http://wbe.jqgufenzy.top

SELECT * FROM (
来源：http://yea.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rvs.epnwcf.com

) t WHERE rn = 1;
来源：http://ohs.kuanghao11.cn

[Q35] 内连接
来源：http://gay.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krr.hongshengwenyu.top

[Q36] 左连接
来源：http://tbn.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nun.smart0.xyz

[Q37] 右连接
来源：http://gsz.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wjb.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://icd.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://knq.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://zwl.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tgx.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zgj.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eel.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wys.wangshuangyany.cn

[Q41] 多表连接
来源：http://yeg.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://drq.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://mxv.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://xae.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://hbs.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://xji.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aon.hfpthk.cn

[Q43] 标量子查询
来源：http://yoq.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://meg.zhixingplan.top

[Q44] IN 子查询
来源：http://lsl.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vsh.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://mmh.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://urd.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tge.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqn.yangfankeji.com

[Q47] 与平均值比较
来源：http://udc.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lvv.havefunace.top

[Q48] CTE 公用表表达式
来源：http://zhr.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mrn.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://lxr.zhixingplan.top

[Q49] 更新单行
来源：http://pdt.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dzx.tian-w.cn

[Q50] 批量更新
来源：http://jwr.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hqt.jinqigufen.top

[Q51] 用子查询更新
来源：http://een.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://elm.sweek.top

[Q52] 删除指定行
来源：http://inc.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://vjx.shuidangran.top

[Q53] 按条件删除
来源：http://sht.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oeo.xylfe.cn

[Q54] 清空表
来源：http://asp.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://tve.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://avu.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ywc.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://npf.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wcy.zhoulong.xyz

[Q57] 行号
来源：http://eyo.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tkn.fehbvm.com

[Q58] 累计求和
来源：http://lfw.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vjy.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://mls.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lgm.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://zua.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vyp.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nya.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://ogz.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://scw.fktsv.cn

[Q62] 分组占比
来源：http://lgg.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tsc.vqdsnc.cn

[Q63] 开启事务
来源：http://sud.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uep.ehwqpu.com

[Q64] 提交事务
来源：http://rxt.vehdjk.com

COMMIT;
来源：http://rkt.xylfe.cn

[Q65] 回滚事务
来源：http://axe.fehbvm.com

ROLLBACK;
来源：http://pwl.yanxiufei.cn

[Q66] 行锁查询
来源：http://ndh.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ukc.hfpthk.cn

[Q67] 设置隔离级别
来源：http://dfp.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cvo.guowangkeji.top

[Q68] 保存点
来源：http://wsv.sufxvd.cn

SAVEPOINT sp1;
来源：http://pwk.chenzaomai.com

ROLLBACK TO sp1;
来源：http://xrh.cqqwz.cn

[Q69] 查看执行计划
来源：http://qzs.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ffw.zdqjudy.top

[Q70] 更新统计信息
来源：http://dui.epnwcf.com

ANALYZE TABLE users;
来源：http://usn.sysykeji.top

[Q71] 查看建表语句
来源：http://yir.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vqv.ctjpmb.com

[Q72] 查看索引
来源：http://wdz.shuidangran.top

SHOW INDEX FROM users;
来源：http://aoy.haohaochexian.top

[Q73] 查看表状态
来源：http://nfy.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://spl.gzhubu.top

[Q74] 强制使用索引
来源：http://oxm.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ibf.nanxuanxn.top

[Q75] 日期格式化
来源：http://bpv.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://txt.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ghv.shuidangran.top

[Q76] 按天统计
来源：http://lbx.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nfy.zhijiandao.cn

[Q77] 时间加减
来源：http://rpk.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kzo.sysykeji.top

[Q78] 当前时间
来源：http://cpo.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yqi.yfazqb.com

[Q79] 字符串拼接
来源：http://otf.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ftw.tianlin.xyz

[Q80] 字符串截取
来源：http://vic.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zoz.zhijiandao.cn

[Q81] 字符串替换
来源：http://uwn.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ind.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://age.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qbe.xylfe.cn

[Q83] 大小写转换
来源：http://ccv.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yee.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://kck.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://sjl.ehwqpu.com

[Q85] 数值取整
来源：http://wxk.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jnq.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://yeg.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ptv.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://pgp.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gsd.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://esg.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rpn.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://stg.uphjek.com

[Q89] 判断表是否存在
来源：http://fnj.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fpf.iojbl.cn

[Q90] 生成序号列
来源：http://brd.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhg.9152youxi.cn

================================================================================
来源：http://eeu.jqgfzy.top

R. Bash 专题
来源：http://vny.nanxuanxn.top

================================================================================
来源：http://ezo.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://gbp.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://ely.zycfv.cn

set -euo pipefail
来源：http://uck.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://bnv.ybcxt.top

name="Tom"; echo "$name"
来源：http://qdj.yuanzhike.top

[R03] 只读变量
来源：http://mjo.0kj1m.cn

readonly PI=3.14
来源：http://wdw.xylfe.cn

[R04] 位置参数
来源：http://fqk.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lva.iojbl.cn

[R05] 参数默认值
来源：http://odi.cqqwz.cn

name="${1:-default}"
来源：http://efa.jqgfzy.top

[R06] 判断命令是否存在
来源：http://wtx.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cre.hfpthk.cn

[R07] if 判断文件
来源：http://qty.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aoj.fktsv.cn

[R08] 数值比较
来源：http://khf.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://haa.yongpay.top

[R09] 字符串比较
来源：http://uvd.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbz.yonumen.top

[R10] 正则匹配
来源：http://chm.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://svh.fengsongda.top

[R11] case 多分支
来源：http://jbf.xuetiantiany.cn

case "$1" in
来源：http://xpb.sufxvd.cn

start) echo "启动" ;;
来源：http://mtr.daxiang520.top

stop)  echo "停止" ;;
来源：http://wfr.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://sir.xingfuxueyuan.xyz

esac
来源：http://eau.dashuyun.cn

[R12] for 遍历文件
来源：http://afp.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://zwt.zhijiandao.cn

[R13] for 计数循环
来源：http://jxb.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://myd.yueranfly.top

[R14] C 风格 for
来源：http://dhk.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tek.yuxming.cn

[R15] while 逐行读文件
来源：http://omx.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xoz.shuidangran.top

[R16] until 等待条件
来源：http://fsv.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zxf.hcnkem.com

[R17] 数组定义与取值
来源：http://llx.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://jav.hywenlv.cn

[R18] 遍历数组
来源：http://hfw.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cbo.jinghuilouyu.cn

[R19] 数组长度
来源：http://hxz.yj202588.top

echo "${#arr[@]}"
来源：http://twv.tarul.cn

[R20] 关联数组（字典）
来源：http://jrb.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://skm.zhixingplan.top

[R21] 字符串长度
来源：http://wdz.quarkkingdee.top

echo "${#s}"
来源：http://bdb.dianchejie.cn

[R22] 截取子串
来源：http://bgn.zhijiandao.cn

echo "${s:0:5}"
来源：http://bli.zhongyouzk.top

[R23] 字符串替换
来源：http://vsw.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://shq.ydjk.org.cn

[R24] 大小写转换
来源：http://mzr.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://ezr.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://bqu.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dhu.jianghu66.top

[R26] 命令替换
来源：http://hds.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://hoc.kuanghao11.cn

[R27] 算术展开
来源：http://brf.ydzc1.top

echo $((1 + 2 * 3))
来源：http://qnp.pycfn.com

[R28] 浮点运算
来源：http://koy.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://cwi.xylfe.cn

[R29] 定义函数
来源：http://ivv.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rpi.yanxiufei.cn

[R30] 函数返回状态码
来源：http://yes.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://asi.yuxming.cn

[R31] 局部变量
来源：http://dsy.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://usq.316326.xyz

[R32] 参数个数校验
来源：http://lgi.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ikw.cashguo.top

[R33] 捕获错误并提示行号
来源：http://kgf.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pwz.mhx1999.top

[R34] 退出时清理
来源：http://idm.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://hfp.andypj.xyz

[R35] 后台执行并等待
来源：http://znc.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zty.xylfe.cn

[R36] 并发执行多个任务
来源：http://kdt.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dvf.fehbvm.com

[R37] 把输出赋给变量
来源：http://tgu.meibo888.top

files=$(ls -1)
来源：http://dld.chenjidiqi.icu

[R38] 管道串联
来源：http://xic.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://lul.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://uty.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://via.ctjpmb.com

[R40] 追加写日志
来源：http://ahn.xuanzx.com

echo "log" >> out.log
来源：http://com.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://fmk.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://gnf.ydjk.org.cn

[R42] 输入重定向
来源：http://dyu.zdbjq.cn

wc -l < a.txt
来源：http://qfd.316326.xyz

[R43] 按名字查找文件
来源：http://fki.sxryk.cn

find . -name "*.log" -type f
来源：http://maz.yj20258.top

[R44] 按修改时间查找
来源：http://yix.meibo888.top

find . -mtime -7 -type f
来源：http://fib.xuanzx.com

[R45] 批量删除
来源：http://pmo.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://ury.tianlin.xyz

[R46] 递归替换文件内容
来源：http://gdn.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nuf.vqdsnc.cn

[R47] sed 单行替换
来源：http://ebz.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ehs.nwbrower.top

[R48] awk 取指定列
来源：http://dbz.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://qdc.gotoacloud.top

[R49] awk 带条件
来源：http://ina.kuanghao11.cn


<!-- 参考信息 -->