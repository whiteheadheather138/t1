代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://giz.xinyue.icu

[Q07] 删除表
来源：http://bti.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://sba.yfazqb.com

[Q08] 创建普通索引
来源：http://nmb.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wlh.fktsv.cn

[Q09] 创建唯一索引
来源：http://lla.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hhu.sjlbkw.cn

[Q10] 插入单行
来源：http://kyl.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tmr.uphjek.com

[Q11] 一次插入多行
来源：http://dqw.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wcn.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://hmv.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lrj.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kos.gogol.net.cn

[Q13] 忽略重复插入
来源：http://fih.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uuh.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://dbh.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zrb.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ibg.yj20258.top

[Q15] 查询全部
来源：http://vsn.havefunace.top

SELECT * FROM users;
来源：http://agm.yfazqb.com

[Q16] 查询指定列
来源：http://rav.ybcxt.top

SELECT id, name FROM users;
来源：http://iyw.hesvh.cn

[Q17] 条件查询
来源：http://cxh.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udc.dianchejie.cn

[Q18] 模糊匹配
来源：http://dtq.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tsc.jinghuilouyu.cn

[Q19] 范围查询
来源：http://wqw.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gtz.fanxiaobao.xyz

[Q20] IN 列表
来源：http://lul.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wnt.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://lhy.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://awi.ydzc1.top

[Q22] 排序
来源：http://jof.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xcd.jlsjyb.cn

[Q23] 分页
来源：http://xmf.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xcv.ehwqpu.com

[Q24] 去重
来源：http://ibe.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://lvg.tianlin.xyz

[Q25] 只取前 N 条
来源：http://ucz.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hly.jlsjyb.cn

[Q26] 计数
来源：http://tnf.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://xdf.bbcook.cn

[Q27] 条件计数
来源：http://dnc.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://edr.snrcjt.cn

[Q28] 求和与平均
来源：http://cyc.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dak.ybcxt.top

[Q29] 最大最小值
来源：http://ogi.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oar.gotoacloud.top

[Q30] 分组统计
来源：http://yvi.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://acr.dashuyun.cn

[Q31] 分组后过滤
来源：http://hhm.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ibi.meibo888.top

[Q32] 分组拼接字符串
来源：http://jwg.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tlg.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kef.smart0.xyz

[Q33] 多列分组
来源：http://yrp.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wco.haohaochexian.top

[Q34] 每组取第一条
来源：http://mlf.hcnkem.com

SELECT * FROM (
来源：http://szk.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mkm.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://chd.gogol.net.cn

[Q35] 内连接
来源：http://ddp.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iyn.yfazqb.com

[Q36] 左连接
来源：http://iuz.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uvn.yj20258888.top

[Q37] 右连接
来源：http://msi.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eks.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://tuh.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jts.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://hmm.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fle.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fiu.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jmz.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ort.svipenyu.cn

[Q41] 多表连接
来源：http://mgc.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://vkt.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://kiz.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://pxy.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://fld.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://khb.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rvh.feifeiyinyue.top

[Q43] 标量子查询
来源：http://wix.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://far.iojbl.cn

[Q44] IN 子查询
来源：http://bkz.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsb.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://czp.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vek.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://wwm.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tsz.nanxuanxn.top

[Q47] 与平均值比较
来源：http://vma.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mrd.pycfn.com

[Q48] CTE 公用表表达式
来源：http://vfv.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nid.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://ehj.zhixingplan.top

[Q49] 更新单行
来源：http://dfe.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://she.nanxinkj.top

[Q50] 批量更新
来源：http://utm.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dko.nanxuanxn.top

[Q51] 用子查询更新
来源：http://yeu.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lnv.tarul.cn

[Q52] 删除指定行
来源：http://gzj.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://rwq.redwolf501.top

[Q53] 按条件删除
来源：http://ste.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eej.smart0.xyz

[Q54] 清空表
来源：http://goi.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://zkn.yj20258888.top

[Q55] 排名（并列占位）
来源：http://taf.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gax.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://gfu.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ktj.jianghu66.top

[Q57] 行号
来源：http://txc.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ipt.zdqjudy.top

[Q58] 累计求和
来源：http://jfe.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://prj.wangshuangyany.cn

[Q59] 分组内累计
来源：http://upr.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lwm.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://fzh.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rxp.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vbk.9152youxi.cn

[Q61] 移动平均
来源：http://elv.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qcz.vqdsnc.cn

[Q62] 分组占比
来源：http://sgc.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fsp.pycfn.com

[Q63] 开启事务
来源：http://seo.0kj1m.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xnb.hfpthk.cn

[Q64] 提交事务
来源：http://cat.xuetiantiany.cn

COMMIT;
来源：http://jsy.jianghu66.top

[Q65] 回滚事务
来源：http://lum.yvedp.cn

ROLLBACK;
来源：http://ppi.zhijiandao.cn

[Q66] 行锁查询
来源：http://fkv.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lyp.cucudq.cn

[Q67] 设置隔离级别
来源：http://sqg.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nmv.yueranfly.top

[Q68] 保存点
来源：http://ncc.fengsongda.top

SAVEPOINT sp1;
来源：http://vny.jianghu66.top

ROLLBACK TO sp1;
来源：http://pyy.birdmap.top

[Q69] 查看执行计划
来源：http://dhu.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vct.shuidangran.top

[Q70] 更新统计信息
来源：http://xdf.aibaodan.cn

ANALYZE TABLE users;
来源：http://fpr.pycfn.com

[Q71] 查看建表语句
来源：http://byo.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yrj.ybcxt.top

[Q72] 查看索引
来源：http://oip.zycfv.cn

SHOW INDEX FROM users;
来源：http://jgy.shangyingyoupin.top

[Q73] 查看表状态
来源：http://pcx.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hoe.chenlongwang.top

[Q74] 强制使用索引
来源：http://wrh.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bkb.zhengqikj.top

[Q75] 日期格式化
来源：http://zwf.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbo.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zkf.vqdsnc.cn

[Q76] 按天统计
来源：http://xeu.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qka.uphjek.com

[Q77] 时间加减
来源：http://svr.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yhn.nwbrower.top

[Q78] 当前时间
来源：http://fad.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fmh.guowangkeji.top

[Q79] 字符串拼接
来源：http://lpp.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hpa.mhx1999.top

[Q80] 字符串截取
来源：http://pic.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yze.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://pgc.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kcp.pycfn.com

[Q82] 字符长度与字节长度
来源：http://nsl.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfu.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://yop.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wui.redwolf501.top

[Q84] 去除首尾空格
来源：http://xym.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://ekd.316326.xyz

[Q85] 数值取整
来源：http://qij.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://svx.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://xla.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kyq.xylfe.cn

[Q87] JSON 字段做条件
来源：http://pbn.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sfm.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://qei.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fkd.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bii.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://gfv.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tko.tarul.cn

[Q90] 生成序号列
来源：http://xsf.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ozp.vqdsnc.cn

================================================================================
来源：http://upp.birdmap.top

R. Bash 专题
来源：http://rmw.sysykeji.top

================================================================================
来源：http://hwp.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://qct.bbcook.cn

#!/usr/bin/env bash
来源：http://dvx.hammf.cn

set -euo pipefail
来源：http://yvw.tanke756.top

[R02] 变量赋值与使用
来源：http://nrf.fengsongda.top

name="Tom"; echo "$name"
来源：http://sen.yvedp.cn

[R03] 只读变量
来源：http://vku.ywan-chungtsiang.top

readonly PI=3.14
来源：http://shq.jqgufenzy.top

[R04] 位置参数
来源：http://mmg.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wws.xziqi.cn

[R05] 参数默认值
来源：http://tlp.sxryk.cn

name="${1:-default}"
来源：http://cmv.zycfv.cn

[R06] 判断命令是否存在
来源：http://cmh.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ltk.yuxming.cn

[R07] if 判断文件
来源：http://hnd.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mop.jinghuilouyu.cn

[R08] 数值比较
来源：http://ddb.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sxt.0kj1m.cn

[R09] 字符串比较
来源：http://wkz.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sfz.zdqjudy.top

[R10] 正则匹配
来源：http://cmg.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wpl.zycfv.cn

[R11] case 多分支
来源：http://kuu.ydjk.org.cn

case "$1" in
来源：http://tto.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://ezj.fehbvm.com

stop)  echo "停止" ;;
来源：http://rnm.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://wrg.zdbjq.cn

esac
来源：http://fog.fengsongda.top

[R12] for 遍历文件
来源：http://gev.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://roz.gotoacloud.top

[R13] for 计数循环
来源：http://jej.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://jue.cucudq.cn

[R14] C 风格 for
来源：http://sbk.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://atv.yj20258.top

[R15] while 逐行读文件
来源：http://jfk.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zvh.daria6918.cn

[R16] until 等待条件
来源：http://dna.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdn.ppjwa.cn

[R17] 数组定义与取值
来源：http://shc.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://lcz.zhixingplan.top

[R18] 遍历数组
来源：http://afa.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rwn.jinghuilouyu.cn

[R19] 数组长度
来源：http://afx.hammf.cn

echo "${#arr[@]}"
来源：http://gha.xylfe.cn

[R20] 关联数组（字典）
来源：http://eao.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iid.jianghu66.top

[R21] 字符串长度
来源：http://zgb.guannengcc.top

echo "${#s}"
来源：http://ufm.xuetiantiany.cn

[R22] 截取子串
来源：http://qic.tanke756.top

echo "${s:0:5}"
来源：http://mza.jinqigufen.top

[R23] 字符串替换
来源：http://aok.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iuk.guowangkeji.top

[R24] 大小写转换
来源：http://fhq.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://xnr.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://lhm.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ern.daria6918.cn

[R26] 命令替换
来源：http://lin.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://iav.bjfxy.top

[R27] 算术展开
来源：http://ppm.shuidangran.top

echo $((1 + 2 * 3))
来源：http://lgq.jlsjyb.cn

[R28] 浮点运算
来源：http://wbr.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://dwt.jianghu66.top

[R29] 定义函数
来源：http://yqa.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xpn.ydjk.org.cn

[R30] 函数返回状态码
来源：http://ubv.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://jnp.bbcook.cn

[R31] 局部变量
来源：http://cef.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://cnt.nwbrower.top

[R32] 参数个数校验
来源：http://ydd.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jjt.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://gpb.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ysb.hywenlv.cn

[R34] 退出时清理
来源：http://poj.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://wpi.hywenlv.cn

[R35] 后台执行并等待
来源：http://azg.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tij.guowangkeji.top

[R36] 并发执行多个任务
来源：http://cqv.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xpm.jyoumei.cn

[R37] 把输出赋给变量
来源：http://yjc.feifeiyinyue.top

files=$(ls -1)
来源：http://xck.yongpay.top

[R38] 管道串联
来源：http://omm.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://iyy.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://xxm.yangfankeji.com

cmd > out.log 2>&1
来源：http://ylz.yj20258888.top

[R40] 追加写日志
来源：http://zer.yangfankeji.com

echo "log" >> out.log
来源：http://hrx.yonumen.top

[R41] 丢弃输出
来源：http://xnf.cashguo.top

cmd >/dev/null 2>&1
来源：http://byg.xylfe.cn

[R42] 输入重定向
来源：http://hfj.bjfxy.top

wc -l < a.txt
来源：http://diu.epnwcf.com

[R43] 按名字查找文件
来源：http://ece.sweek.top

find . -name "*.log" -type f
来源：http://vhf.redwolf501.top

[R44] 按修改时间查找
来源：http://pol.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://yew.xziqi.cn

[R45] 批量删除
来源：http://spn.bbcook.cn

find . -name "*.tmp" -delete
来源：http://xek.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://pdk.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gmv.sweek.top

[R47] sed 单行替换
来源：http://dql.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://doy.0kj1m.cn

[R48] awk 取指定列
来源：http://vcr.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://qpg.haohaochexian.top

[R49] awk 带条件
来源：http://rkf.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lky.ydjk.org.cn

[R50] awk 求和
来源：http://qms.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ccu.tian-w.cn

[R51] 排序去重取前几
来源：http://icc.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qua.ybcxt.top

[R52] 统计行数
来源：http://ian.wangdashe.top

wc -l a.txt
来源：http://pwh.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://chc.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://igi.pengpengdd.cyou

[R54] 比较两个文件
来源：http://akt.gotoacloud.top

diff a.txt b.txt
来源：http://prw.meibo888.top

[R55] 压缩与解压
来源：http://ptz.quarkkingdee.top


<!-- 参考信息 -->