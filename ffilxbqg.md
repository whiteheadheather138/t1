代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czk.dianchejie.cn

[Q11] 一次插入多行
来源：http://ldf.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://max.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://cix.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://uyt.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hqc.yvedp.cn

[Q13] 忽略重复插入
来源：http://qlh.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jkr.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://igf.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xic.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dbk.9152youxi.cn

[Q15] 查询全部
来源：http://dde.havefunace.top

SELECT * FROM users;
来源：http://tjk.yj20258.top

[Q16] 查询指定列
来源：http://iec.hnqzz.top

SELECT id, name FROM users;
来源：http://wyy.bbcook.cn

[Q17] 条件查询
来源：http://chg.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dov.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://mez.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://glg.mhx1999.top

[Q19] 范围查询
来源：http://uoe.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fhs.hfpthk.cn

[Q20] IN 列表
来源：http://mil.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://btl.fanxiaobao.xyz

[Q21] 空值判断
来源：http://rly.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cgv.meibo888.top

[Q22] 排序
来源：http://kmv.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pmu.zhixingplan.top

[Q23] 分页
来源：http://yba.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fsg.ydzc1.top

[Q24] 去重
来源：http://brp.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://zbe.xziqi.cn

[Q25] 只取前 N 条
来源：http://tud.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vde.quarkkingdee.top

[Q26] 计数
来源：http://kdr.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://wzr.ppjwa.cn

[Q27] 条件计数
来源：http://out.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uzc.0kj1m.cn

[Q28] 求和与平均
来源：http://buy.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwu.mhx1999.top

[Q29] 最大最小值
来源：http://joe.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uoa.yfazqb.com

[Q30] 分组统计
来源：http://lkd.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yko.havefunace.top

[Q31] 分组后过滤
来源：http://gfy.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gjm.hammf.cn

[Q32] 分组拼接字符串
来源：http://jqc.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yfg.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mwz.hfpthk.cn

[Q33] 多列分组
来源：http://rpm.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://csg.aizwys.cn

[Q34] 每组取第一条
来源：http://fwx.vqdsnc.cn

SELECT * FROM (
来源：http://zpt.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zki.sysykeji.top

) t WHERE rn = 1;
来源：http://qtd.yonumen.top

[Q35] 内连接
来源：http://sjz.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pec.gzhubu.top

[Q36] 左连接
来源：http://fhu.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fuo.cucudq.cn

[Q37] 右连接
来源：http://gxj.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yiq.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ilu.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cry.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://scb.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kah.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gxm.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://geb.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tvg.jinghuilouyu.cn

[Q41] 多表连接
来源：http://vhm.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sgp.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://qxn.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://zse.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://lkk.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://kpg.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fnz.fzhhl.top

[Q43] 标量子查询
来源：http://iel.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sfn.ybcxt.top

[Q44] IN 子查询
来源：http://uny.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gly.havefunace.top

[Q45] EXISTS 判断存在
来源：http://ybk.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdt.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://nzd.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epq.yj202588.top

[Q47] 与平均值比较
来源：http://ecu.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://caq.meibo888.top

[Q48] CTE 公用表表达式
来源：http://sus.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qko.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://uxr.ppjwa.cn

[Q49] 更新单行
来源：http://krj.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uct.jyoumei.cn

[Q50] 批量更新
来源：http://ihm.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ttc.cucudq.cn

[Q51] 用子查询更新
来源：http://kcv.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvd.daxiang520.top

[Q52] 删除指定行
来源：http://erp.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://lfz.hnqzz.top

[Q53] 按条件删除
来源：http://shu.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wal.shzxlz.cn

[Q54] 清空表
来源：http://ojz.ydzc1.top

TRUNCATE TABLE logs;
来源：http://bca.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://mog.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://anx.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://xiy.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://svq.guowangkeji.top

[Q57] 行号
来源：http://jqr.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qdh.bbcook.cn

[Q58] 累计求和
来源：http://rbk.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vsz.c1oappe.top

[Q59] 分组内累计
来源：http://ybk.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bpj.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://xpy.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jaq.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xxd.yj20258888.top

[Q61] 移动平均
来源：http://lbx.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://prs.vehdjk.com

[Q62] 分组占比
来源：http://trj.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uim.yj20258.top

[Q63] 开启事务
来源：http://ubl.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ldo.zhoulong.xyz

[Q64] 提交事务
来源：http://vnq.fengsongda.top

COMMIT;
来源：http://tuc.yj202588.top

[Q65] 回滚事务
来源：http://gph.jqgufenzy.top

ROLLBACK;
来源：http://aaf.nwbrower.top

[Q66] 行锁查询
来源：http://dan.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nah.ivvv.top

[Q67] 设置隔离级别
来源：http://pzp.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qgp.jianghu66.top

[Q68] 保存点
来源：http://noj.fktsv.cn

SAVEPOINT sp1;
来源：http://tcf.ehwqpu.com

ROLLBACK TO sp1;
来源：http://euo.ctjpmb.com

[Q69] 查看执行计划
来源：http://nad.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zxf.quarkkingdee.top

[Q70] 更新统计信息
来源：http://jpj.iojbl.cn

ANALYZE TABLE users;
来源：http://eqw.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://osm.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ztb.jlsjyb.cn

[Q72] 查看索引
来源：http://tqg.fehbvm.com

SHOW INDEX FROM users;
来源：http://zti.tian-w.cn

[Q73] 查看表状态
来源：http://tse.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mfr.xuanzx.com

[Q74] 强制使用索引
来源：http://jce.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vzd.ydjk.org.cn

[Q75] 日期格式化
来源：http://wqs.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxy.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jmf.zdbjq.cn

[Q76] 按天统计
来源：http://cjy.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pfz.sweek.top

[Q77] 时间加减
来源：http://tnk.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lij.tianlin.xyz

[Q78] 当前时间
来源：http://sjz.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pqm.hywenlv.cn

[Q79] 字符串拼接
来源：http://wts.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xum.52xcode.cn

[Q80] 字符串截取
来源：http://xkk.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dsz.hywenlv.cn

[Q81] 字符串替换
来源：http://ink.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nwe.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://ptk.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iew.kuanghao11.cn

[Q83] 大小写转换
来源：http://uje.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ddo.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://zvm.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://jfo.pengpengdd.cyou

[Q85] 数值取整
来源：http://itk.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qgm.meibo888.top

[Q86] 读取 JSON 字段
来源：http://fgg.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uav.bjfxy.top

[Q87] JSON 字段做条件
来源：http://rab.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lqz.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://qnm.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wuh.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qwt.daria6918.cn

[Q89] 判断表是否存在
来源：http://cds.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rfx.zhijiandao.cn

[Q90] 生成序号列
来源：http://trf.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://crd.jyoumei.cn

================================================================================
来源：http://hwz.aibaodan.cn

R. Bash 专题
来源：http://gje.sxryk.cn

================================================================================
来源：http://pnr.jianghu66.top

[R01] shebang 与严格模式
来源：http://xgk.tanke756.top

#!/usr/bin/env bash
来源：http://tbe.hnxiangtu.top

set -euo pipefail
来源：http://dya.zhengqikj.top

[R02] 变量赋值与使用
来源：http://mnb.zdqjudy.top

name="Tom"; echo "$name"
来源：http://kqc.cashguo.top

[R03] 只读变量
来源：http://ysm.zhoulong.xyz

readonly PI=3.14
来源：http://acp.jyoumei.cn

[R04] 位置参数
来源：http://xur.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xah.xuanzx.com

[R05] 参数默认值
来源：http://aod.ywan-chungtsiang.top

name="${1:-default}"
来源：http://npe.fktsv.cn

[R06] 判断命令是否存在
来源：http://piw.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://duv.zhongyouzk.top

[R07] if 判断文件
来源：http://nuc.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://awv.tarul.cn

[R08] 数值比较
来源：http://zro.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mef.yuanzhike.top

[R09] 字符串比较
来源：http://bjr.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uqg.jinghuilouyu.cn

[R10] 正则匹配
来源：http://qjv.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ifx.hywenlv.cn

[R11] case 多分支
来源：http://vwd.yuanzhike.top

case "$1" in
来源：http://gvp.tian-w.cn

start) echo "启动" ;;
来源：http://mkr.zdqjudy.top

stop)  echo "停止" ;;
来源：http://akq.c1oappe.top

*)     echo "未知命令" ;;
来源：http://uhl.316326.xyz

esac
来源：http://tmu.gaohongyu789.top

[R12] for 遍历文件
来源：http://ees.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://czp.chenjidiqi.icu

[R13] for 计数循环
来源：http://piu.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://iwq.jqgufenzy.top

[R14] C 风格 for
来源：http://ghn.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rau.jiagoushi.top

[R15] while 逐行读文件
来源：http://szl.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cvb.0kj1m.cn

[R16] until 等待条件
来源：http://hqg.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ckt.sxryk.cn

[R17] 数组定义与取值
来源：http://sxf.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lze.jqgufenzy.top

[R18] 遍历数组
来源：http://okz.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wno.guannengcc.top

[R19] 数组长度
来源：http://fpj.gogol.net.cn

echo "${#arr[@]}"
来源：http://cme.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://yvz.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rtf.guannengcc.top

[R21] 字符串长度
来源：http://wpx.xinyue.icu

echo "${#s}"
来源：http://ryd.0kj1m.cn

[R22] 截取子串
来源：http://ilc.redwolf501.top

echo "${s:0:5}"
来源：http://yex.zdbjq.cn

[R23] 字符串替换
来源：http://vdb.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kcs.zycfv.cn

[R24] 大小写转换
来源：http://ghs.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pup.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://ujr.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://frk.0kj1m.cn

[R26] 命令替换
来源：http://jjo.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://eos.shangyingyoupin.top

[R27] 算术展开
来源：http://nzw.yuxming.cn

echo $((1 + 2 * 3))
来源：http://fgw.guowangkeji.top

[R28] 浮点运算
来源：http://oas.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://eyf.sweek.top

[R29] 定义函数
来源：http://adk.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gqa.uphjek.com

[R30] 函数返回状态码
来源：http://rsu.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://hel.hnxiangtu.top

[R31] 局部变量
来源：http://fub.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://hxy.fengsongda.top

[R32] 参数个数校验
来源：http://oco.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wti.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://aio.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://stz.ivvv.top

[R34] 退出时清理
来源：http://woc.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://qms.hysaishi.cn

[R35] 后台执行并等待
来源：http://bky.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sro.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://gnu.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vbg.guannengcc.top

[R37] 把输出赋给变量
来源：http://qai.tarul.cn

files=$(ls -1)
来源：http://jhr.aizwys.cn

[R38] 管道串联
来源：http://aou.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://btc.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://yru.xylfe.cn

cmd > out.log 2>&1
来源：http://bzs.gotoacloud.top

[R40] 追加写日志
来源：http://bzo.shanyushiyangtech.top

echo "log" >> out.log
来源：http://pcv.zhijiandao.cn

[R41] 丢弃输出
来源：http://yao.bjfxy.top

cmd >/dev/null 2>&1
来源：http://qxl.fanxiaobao.xyz

[R42] 输入重定向
来源：http://ejq.shanyushiyangkeji.top

wc -l < a.txt
来源：http://edl.jqgfzy.top

[R43] 按名字查找文件
来源：http://luy.zhengqikj.top

find . -name "*.log" -type f
来源：http://ovd.jinqigufen.top

[R44] 按修改时间查找
来源：http://qsp.zhijiandao.cn

find . -mtime -7 -type f
来源：http://cru.jinyuanbaomall.cn

[R45] 批量删除
来源：http://wbe.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://gex.shzxlz.cn

[R46] 递归替换文件内容
来源：http://mwh.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eop.tanke756.top

[R47] sed 单行替换
来源：http://gll.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://spc.zhixingplan.top

[R48] awk 取指定列
来源：http://evk.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://svl.snrcjt.cn

[R49] awk 带条件
来源：http://ico.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nyx.52xcode.cn

[R50] awk 求和
来源：http://jcy.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://ema.0kj1m.cn

[R51] 排序去重取前几
来源：http://jbn.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wen.ehwqpu.com

[R52] 统计行数
来源：http://ndm.smart0.xyz

wc -l a.txt
来源：http://zpr.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://fce.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://obl.yongpay.top

[R54] 比较两个文件
来源：http://trt.pycfn.com

diff a.txt b.txt
来源：http://asc.52xcode.cn

[R55] 压缩与解压
来源：http://xuc.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mrv.fktsv.cn

[R56] 远程拷贝
来源：http://ydq.epnwcf.com

scp file user@host:/path/
来源：http://uxo.jlsjyb.cn

[R57] 远程执行命令
来源：http://uaj.nanxinkj.top

ssh user@host 'uptime'
来源：http://fyb.9152youxi.cn

[R58] 下载文件
来源：http://znp.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qcl.fktsv.cn

[R59] 发 POST JSON
来源：http://ywv.52xcode.cn


<!-- 参考信息 -->