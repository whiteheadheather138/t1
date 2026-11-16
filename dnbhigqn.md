代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://xlz.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kcm.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://aku.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yes.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://tbo.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zoo.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsv.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://qpr.jqgfzy.top

SELECT * FROM users;
来源：http://qra.fehbvm.com

[Q16] 查询指定列
来源：http://qpa.hammf.cn

SELECT id, name FROM users;
来源：http://mhi.daxiang520.top

[Q17] 条件查询
来源：http://vik.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wiz.nanxuanxn.top

[Q18] 模糊匹配
来源：http://pej.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://erk.ydjk.org.cn

[Q19] 范围查询
来源：http://nkc.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lgs.chenzaomai.com

[Q20] IN 列表
来源：http://cjf.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ita.ctjpmb.com

[Q21] 空值判断
来源：http://pmi.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dws.jiagoushi.top

[Q22] 排序
来源：http://bfs.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fpm.zhiwuduotai.top

[Q23] 分页
来源：http://qwg.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iqj.c1oappe.top

[Q24] 去重
来源：http://sag.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://psc.tanke756.top

[Q25] 只取前 N 条
来源：http://moe.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bks.nwbrower.top

[Q26] 计数
来源：http://enk.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://lqa.fktsv.cn

[Q27] 条件计数
来源：http://nfn.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qdv.vqdsnc.cn

[Q28] 求和与平均
来源：http://yzw.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xza.fzhhl.top

[Q29] 最大最小值
来源：http://uqt.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rhr.quarkkingdee.top

[Q30] 分组统计
来源：http://asn.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wfg.yanxiufei.cn

[Q31] 分组后过滤
来源：http://dez.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ahe.shuidangran.top

[Q32] 分组拼接字符串
来源：http://akh.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxb.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ioj.hywenlv.cn

[Q33] 多列分组
来源：http://xfg.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bdo.yangfankeji.com

[Q34] 每组取第一条
来源：http://mng.zdbjq.cn

SELECT * FROM (
来源：http://jgl.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gwn.redwolf501.top

) t WHERE rn = 1;
来源：http://zkx.birdmap.top

[Q35] 内连接
来源：http://oty.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ggh.xylfe.cn

[Q36] 左连接
来源：http://dch.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jfj.tarul.cn

[Q37] 右连接
来源：http://sfl.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xkx.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://oiu.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qbv.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://pzc.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fsr.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://anw.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dwm.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vae.yuanzhike.top

[Q41] 多表连接
来源：http://kqv.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zoe.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://kga.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://fms.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://oqv.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://ami.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ihh.birdmap.top

[Q43] 标量子查询
来源：http://acj.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kwx.shangyingyoupin.top

[Q44] IN 子查询
来源：http://wdd.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pjy.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://uen.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://esy.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://gpw.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xei.hfpthk.cn

[Q47] 与平均值比较
来源：http://ztf.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://drk.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://qll.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xdv.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://pwd.mhx1999.top

[Q49] 更新单行
来源：http://yjs.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aht.0kj1m.cn

[Q50] 批量更新
来源：http://ryr.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lxs.sweek.top

[Q51] 用子查询更新
来源：http://vdv.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://meu.yuanzhike.top

[Q52] 删除指定行
来源：http://giw.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://fru.cheryme.top

[Q53] 按条件删除
来源：http://zyd.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yvp.tian-w.cn

[Q54] 清空表
来源：http://xql.hesvh.cn

TRUNCATE TABLE logs;
来源：http://tkk.fzhhl.top

[Q55] 排名（并列占位）
来源：http://kcm.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://epv.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://gbg.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yep.shanyushiyangkeji.top

[Q57] 行号
来源：http://emf.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hdr.shangyingyoupin.top

[Q58] 累计求和
来源：http://wow.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tnn.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://snn.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jhs.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://jdf.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cje.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cft.iojbl.cn

[Q61] 移动平均
来源：http://sut.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://txr.9152youxi.cn

[Q62] 分组占比
来源：http://qqt.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uid.ppjwa.cn

[Q63] 开启事务
来源：http://bhl.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tfg.tianlin.xyz

[Q64] 提交事务
来源：http://jyi.xingfuxueyuan.xyz

COMMIT;
来源：http://kje.ydjk.org.cn

[Q65] 回滚事务
来源：http://sdi.smart0.xyz

ROLLBACK;
来源：http://glc.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://dba.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qth.fzhhl.top

[Q67] 设置隔离级别
来源：http://pcb.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ios.hfpthk.cn

[Q68] 保存点
来源：http://pia.ivvv.top

SAVEPOINT sp1;
来源：http://xtn.andypj.xyz

ROLLBACK TO sp1;
来源：http://wtx.sysykeji.top

[Q69] 查看执行计划
来源：http://cjh.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lva.gotoacloud.top

[Q70] 更新统计信息
来源：http://usp.shangyingyoupin.top

ANALYZE TABLE users;
来源：http://xat.epnwcf.com

[Q71] 查看建表语句
来源：http://jbk.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mas.xuanzx.com

[Q72] 查看索引
来源：http://cmg.hcnkem.com

SHOW INDEX FROM users;
来源：http://ndv.meibo888.top

[Q73] 查看表状态
来源：http://aqx.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tmm.gaohongyu789.top

[Q74] 强制使用索引
来源：http://rll.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wer.jinqigufen.top

[Q75] 日期格式化
来源：http://puw.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tdo.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bbv.jiagoushi.top

[Q76] 按天统计
来源：http://lxp.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pal.ehwqpu.com

[Q77] 时间加减
来源：http://sty.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nsr.gaohongyu789.top

[Q78] 当前时间
来源：http://zqa.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hrg.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://lcf.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kkd.daxiang520.top

[Q80] 字符串截取
来源：http://oje.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qld.nanxinkj.top

[Q81] 字符串替换
来源：http://tte.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pgb.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://cmh.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ulg.smart0.xyz

[Q83] 大小写转换
来源：http://hpf.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cqs.cashguo.top

[Q84] 去除首尾空格
来源：http://yva.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://etc.shangyingyoupin.top

[Q85] 数值取整
来源：http://ifn.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jir.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://yub.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ssn.yongpay.top

[Q87] JSON 字段做条件
来源：http://aid.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vbd.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://sec.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lsb.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zlk.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://ufl.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ios.cqqwz.cn

[Q90] 生成序号列
来源：http://kha.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pns.bbcook.cn

================================================================================
来源：http://rii.hnxiangtu.top

R. Bash 专题
来源：http://jrs.aizwys.cn

================================================================================
来源：http://vyo.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://cuy.ydjk.org.cn

#!/usr/bin/env bash
来源：http://plc.hywenlv.cn

set -euo pipefail
来源：http://oxo.cdnleiting.top

[R02] 变量赋值与使用
来源：http://rky.9152youxi.cn

name="Tom"; echo "$name"
来源：http://kjk.jianghu66.top

[R03] 只读变量
来源：http://skt.shuidangran.top

readonly PI=3.14
来源：http://ygv.316326.xyz

[R04] 位置参数
来源：http://ezx.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lrh.jqgufenzy.top

[R05] 参数默认值
来源：http://coo.tarul.cn

name="${1:-default}"
来源：http://sbn.zhixingplan.top

[R06] 判断命令是否存在
来源：http://jys.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dho.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://hdl.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jtj.dianchejie.cn

[R08] 数值比较
来源：http://ogk.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jen.nanxinkj.top

[R09] 字符串比较
来源：http://bfd.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fgg.snrcjt.cn

[R10] 正则匹配
来源：http://ofz.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lvq.snrcjt.cn

[R11] case 多分支
来源：http://mkw.wangshuangyany.cn

case "$1" in
来源：http://ezh.svipenyu.cn

start) echo "启动" ;;
来源：http://xqz.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://pri.ivvv.top

*)     echo "未知命令" ;;
来源：http://vlu.cucudq.cn

esac
来源：http://ujc.yj20258888.top

[R12] for 遍历文件
来源：http://nku.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://dyp.nanxinkj.top

[R13] for 计数循环
来源：http://ost.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://yiv.jqgfzy.top

[R14] C 风格 for
来源：http://acd.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aie.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://dcc.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://miw.feifeiyinyue.top

[R16] until 等待条件
来源：http://zrx.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://poi.bbcook.cn

[R17] 数组定义与取值
来源：http://eej.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yev.zhiwuduotai.top

[R18] 遍历数组
来源：http://cnl.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jnd.daxiang520.top

[R19] 数组长度
来源：http://are.pycfn.com

echo "${#arr[@]}"
来源：http://wfu.yuxming.cn

[R20] 关联数组（字典）
来源：http://fgg.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ark.0kj1m.cn

[R21] 字符串长度
来源：http://dwe.epnwcf.com

echo "${#s}"
来源：http://pqe.cheryme.top

[R22] 截取子串
来源：http://lsa.jqgfzy.top

echo "${s:0:5}"
来源：http://saz.ppjwa.cn

[R23] 字符串替换
来源：http://ial.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mjw.yfazqb.com

[R24] 大小写转换
来源：http://red.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://ugf.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://lrm.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fmt.sufxvd.cn

[R26] 命令替换
来源：http://wfy.havefunace.top

now=$(date +%F); echo "$now"
来源：http://awb.yvedp.cn

[R27] 算术展开
来源：http://zha.fehbvm.com

echo $((1 + 2 * 3))
来源：http://fiv.zycfv.cn

[R28] 浮点运算
来源：http://wrw.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://nfh.bbcook.cn

[R29] 定义函数
来源：http://ucy.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lrj.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://czm.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://rlz.yfazqb.com

[R31] 局部变量
来源：http://rjc.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://fvy.yuanzhike.top

[R32] 参数个数校验
来源：http://whv.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fou.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://rnm.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iaa.tarul.cn

[R34] 退出时清理
来源：http://kmk.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qdg.xinyue.icu

[R35] 后台执行并等待
来源：http://cjh.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hsc.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://ryk.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://quv.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://ndr.epnwcf.com

files=$(ls -1)
来源：http://wcj.yj20258888.top

[R38] 管道串联
来源：http://bsv.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://ghc.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://kte.316326.xyz

cmd > out.log 2>&1
来源：http://lbi.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://svh.zycfv.cn

echo "log" >> out.log
来源：http://qde.hywenlv.cn

[R41] 丢弃输出
来源：http://dta.pycfn.com

cmd >/dev/null 2>&1
来源：http://eep.zhongyouzk.top

[R42] 输入重定向
来源：http://ekp.aibaodan.cn

wc -l < a.txt
来源：http://fwg.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://lye.cashguo.top

find . -name "*.log" -type f
来源：http://hzo.gaohongyu789.top

[R44] 按修改时间查找
来源：http://wak.cqqwz.cn

find . -mtime -7 -type f
来源：http://qld.hcnkem.com

[R45] 批量删除
来源：http://hlh.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://epc.andypj.xyz

[R46] 递归替换文件内容
来源：http://ztj.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://evw.jyoumei.cn

[R47] sed 单行替换
来源：http://lfb.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hxu.aibaodan.cn

[R48] awk 取指定列
来源：http://vtn.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://ufm.hywenlv.cn

[R49] awk 带条件
来源：http://fzu.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sml.fzhhl.top

[R50] awk 求和
来源：http://wxn.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://hep.nanxinkj.top

[R51] 排序去重取前几
来源：http://sbc.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://uki.nanxuanxn.top

[R52] 统计行数
来源：http://yfx.yfazqb.com

wc -l a.txt
来源：http://cgx.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://oqy.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gfb.aizwys.cn

[R54] 比较两个文件
来源：http://kps.pengpengdd.cyou

diff a.txt b.txt
来源：http://dqk.yj20258888.top

[R55] 压缩与解压
来源：http://eaz.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xoa.quarkkingdee.top

[R56] 远程拷贝
来源：http://zbm.c1oappe.top

scp file user@host:/path/
来源：http://fxd.yuanzhike.top

[R57] 远程执行命令
来源：http://jnq.gogol.net.cn

ssh user@host 'uptime'
来源：http://mlg.fehbvm.com

[R58] 下载文件
来源：http://ofj.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://amj.sufxvd.cn

[R59] 发 POST JSON
来源：http://hfc.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://exu.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://ydt.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ecd.jianghu66.top

[R61] 磁盘占用
来源：http://wjc.jyoumei.cn


<!-- 参考信息 -->