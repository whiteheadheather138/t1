代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://dec.ehwqpu.com

[Q09] 创建唯一索引
来源：http://ope.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://van.zhixingplan.top

[Q10] 插入单行
来源：http://dua.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fpn.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://bgg.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vut.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://pjp.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://wyo.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lry.uphjek.com

[Q13] 忽略重复插入
来源：http://qkz.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hiz.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://jpv.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rgr.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tda.hywenlv.cn

[Q15] 查询全部
来源：http://lln.chenlongwang.top

SELECT * FROM users;
来源：http://yip.gaohongyu789.top

[Q16] 查询指定列
来源：http://gbc.zycfv.cn

SELECT id, name FROM users;
来源：http://xsj.svipenyu.cn

[Q17] 条件查询
来源：http://fct.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wlc.jinqigfzy.top

[Q18] 模糊匹配
来源：http://qog.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cno.jianghu66.top

[Q19] 范围查询
来源：http://rlo.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mjy.fengsongda.top

[Q20] IN 列表
来源：http://qdt.kuanghao11.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ial.chenjidiqi.icu

[Q21] 空值判断
来源：http://mdu.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://prb.epnwcf.com

[Q22] 排序
来源：http://awb.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zuq.zhixingplan.top

[Q23] 分页
来源：http://dhh.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzg.shanyushiyangkeji.top

[Q24] 去重
来源：http://zrz.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://krt.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://lsn.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mhi.jiagoushi.top

[Q26] 计数
来源：http://fny.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://svi.sxryk.cn

[Q27] 条件计数
来源：http://bsb.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cys.zhiwuduotai.top

[Q28] 求和与平均
来源：http://dfl.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yct.snrcjt.cn

[Q29] 最大最小值
来源：http://wrq.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://umb.yangfankeji.com

[Q30] 分组统计
来源：http://azj.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dzk.yvedp.cn

[Q31] 分组后过滤
来源：http://cuk.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ors.52xcode.cn

[Q32] 分组拼接字符串
来源：http://whg.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kxj.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yaa.gzhubu.top

[Q33] 多列分组
来源：http://soz.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mue.ppjwa.cn

[Q34] 每组取第一条
来源：http://wvf.tarul.cn

SELECT * FROM (
来源：http://nxz.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bwq.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://aok.tarul.cn

[Q35] 内连接
来源：http://mhk.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jxi.ppjwa.cn

[Q36] 左连接
来源：http://xqu.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nwt.hnqzz.top

[Q37] 右连接
来源：http://gxx.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eqk.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://era.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eju.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://afg.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://adc.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ohz.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cwf.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xub.xuanzx.com

[Q41] 多表连接
来源：http://qux.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wif.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://hbd.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://plm.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://eeh.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://bec.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qyh.xziqi.cn

[Q43] 标量子查询
来源：http://txc.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://izu.feifeiyinyue.top

[Q44] IN 子查询
来源：http://onz.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wjg.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://eqq.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dew.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://ojo.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqp.fengsongda.top

[Q47] 与平均值比较
来源：http://ksr.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hoz.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://spw.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qpl.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://qfb.tarul.cn

[Q49] 更新单行
来源：http://tdq.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fvk.jqgufenzy.top

[Q50] 批量更新
来源：http://yif.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cgx.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://mae.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yfa.zdqjudy.top

[Q52] 删除指定行
来源：http://szx.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://nkv.dianchejie.cn

[Q53] 按条件删除
来源：http://jwz.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mqr.yongpay.top

[Q54] 清空表
来源：http://fwe.iojbl.cn

TRUNCATE TABLE logs;
来源：http://hiq.bjfxy.top

[Q55] 排名（并列占位）
来源：http://cud.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ild.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://qgi.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pnr.tarul.cn

[Q57] 行号
来源：http://eks.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://efx.vehdjk.com

[Q58] 累计求和
来源：http://lhz.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://prl.nanxuanxn.top

[Q59] 分组内累计
来源：http://gsc.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://myb.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://pdf.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://viz.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bjd.svipenyu.cn

[Q61] 移动平均
来源：http://btx.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zou.daxiang520.top

[Q62] 分组占比
来源：http://hio.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://paz.fengsongda.top

[Q63] 开启事务
来源：http://knk.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://epn.chenjidiqi.icu

[Q64] 提交事务
来源：http://trl.havefunace.top

COMMIT;
来源：http://caw.zhiwuduotai.top

[Q65] 回滚事务
来源：http://wew.bbcook.cn

ROLLBACK;
来源：http://yjh.zhiwuduotai.top

[Q66] 行锁查询
来源：http://dor.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iau.uphjek.com

[Q67] 设置隔离级别
来源：http://vuz.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lih.sysykeji.top

[Q68] 保存点
来源：http://ltm.bbcook.cn

SAVEPOINT sp1;
来源：http://pvz.zhengqikj.top

ROLLBACK TO sp1;
来源：http://qcp.zdqjudy.top

[Q69] 查看执行计划
来源：http://wdy.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tnf.gogol.net.cn

[Q70] 更新统计信息
来源：http://xka.hysaishi.cn

ANALYZE TABLE users;
来源：http://bks.yangfankeji.com

[Q71] 查看建表语句
来源：http://eeq.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fzp.ctjpmb.com

[Q72] 查看索引
来源：http://vkj.yuanzhike.top

SHOW INDEX FROM users;
来源：http://nda.yanxiufei.cn

[Q73] 查看表状态
来源：http://jop.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dfb.quarkkingdee.top

[Q74] 强制使用索引
来源：http://drb.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xbz.yj20258.top

[Q75] 日期格式化
来源：http://pwq.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yvk.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egg.cashguo.top

[Q76] 按天统计
来源：http://goq.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ajq.andypj.xyz

[Q77] 时间加减
来源：http://veg.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jsc.pengpengdd.cyou

[Q78] 当前时间
来源：http://gvt.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cjd.ehwqpu.com

[Q79] 字符串拼接
来源：http://xcp.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tas.hcnkem.com

[Q80] 字符串截取
来源：http://lhe.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lln.svipenyu.cn

[Q81] 字符串替换
来源：http://fkt.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zrh.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://jfq.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zcr.kuanghao11.cn

[Q83] 大小写转换
来源：http://ddp.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ftl.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://gct.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://iij.jiagoushi.top

[Q85] 数值取整
来源：http://tfn.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dnm.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://jgb.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://czd.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://bfs.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vfd.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://ems.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sjv.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ciz.zhengqikj.top

[Q89] 判断表是否存在
来源：http://nmd.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ffu.wangshuangyany.cn

[Q90] 生成序号列
来源：http://wlj.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pqo.daxiang520.top

================================================================================
来源：http://wty.cucudq.cn

R. Bash 专题
来源：http://yac.snrcjt.cn

================================================================================
来源：http://oiz.yangfankeji.com

[R01] shebang 与严格模式
来源：http://svf.kuanghao11.cn

#!/usr/bin/env bash
来源：http://mcv.tarul.cn

set -euo pipefail
来源：http://yhj.nanxinkj.top

[R02] 变量赋值与使用
来源：http://tav.zycfv.cn

name="Tom"; echo "$name"
来源：http://uqq.hongshengwenyu.top

[R03] 只读变量
来源：http://snf.cashguo.top

readonly PI=3.14
来源：http://bzg.bjfxy.top

[R04] 位置参数
来源：http://jbv.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mzo.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://ybf.tianlin.xyz

name="${1:-default}"
来源：http://lke.316326.xyz

[R06] 判断命令是否存在
来源：http://gur.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nkr.zhengqikj.top

[R07] if 判断文件
来源：http://jku.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://edt.shangyingyoupin.top

[R08] 数值比较
来源：http://hbf.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vbb.52xcode.cn

[R09] 字符串比较
来源：http://ztf.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zmo.nanxinkj.top

[R10] 正则匹配
来源：http://grc.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gzy.svipenyu.cn

[R11] case 多分支
来源：http://xjz.yueranfly.top

case "$1" in
来源：http://alc.yfazqb.com

start) echo "启动" ;;
来源：http://dfs.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://yor.epnwcf.com

*)     echo "未知命令" ;;
来源：http://xjq.jinqigfzy.top

esac
来源：http://aps.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://zoo.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://vwl.xziqi.cn

[R13] for 计数循环
来源：http://vns.feifeiyinyue.top

for i in {1..10}; do echo "$i"; done
来源：http://anr.tarul.cn

[R14] C 风格 for
来源：http://thd.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yls.snrcjt.cn

[R15] while 逐行读文件
来源：http://crv.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rlc.zhoulong.xyz

[R16] until 等待条件
来源：http://hxq.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://woh.yueranfly.top

[R17] 数组定义与取值
来源：http://kjg.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://rvi.zhengqikj.top

[R18] 遍历数组
来源：http://kam.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pog.yonumen.top

[R19] 数组长度
来源：http://wnj.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://vum.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://azm.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tbj.yj202588.top

[R21] 字符串长度
来源：http://avu.wangdashe.top

echo "${#s}"
来源：http://zng.52xcode.cn

[R22] 截取子串
来源：http://xiz.sxryk.cn

echo "${s:0:5}"
来源：http://ymz.ehwqpu.com

[R23] 字符串替换
来源：http://buy.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xew.redwolf501.top

[R24] 大小写转换
来源：http://olc.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://zuu.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://zdo.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://etk.kuanghao11.cn

[R26] 命令替换
来源：http://vki.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://zch.ehwqpu.com

[R27] 算术展开
来源：http://tmr.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://wop.dashuyun.cn

[R28] 浮点运算
来源：http://cmf.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://flb.shuidangran.top

[R29] 定义函数
来源：http://hbp.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pph.fengsongda.top

[R30] 函数返回状态码
来源：http://dnf.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://qjy.andypj.xyz

[R31] 局部变量
来源：http://wzw.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://dws.ivvv.top

[R32] 参数个数校验
来源：http://kcg.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gso.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://rws.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ewu.yueranfly.top

[R34] 退出时清理
来源：http://xgf.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aeo.vehdjk.com

[R35] 后台执行并等待
来源：http://vag.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ywl.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://jtz.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qyy.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://nob.yj20258888.top

files=$(ls -1)
来源：http://rqi.vehdjk.com

[R38] 管道串联
来源：http://vdw.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://gey.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://vwz.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://mec.fzhhl.top

[R40] 追加写日志
来源：http://isu.jqgufenzy.top

echo "log" >> out.log
来源：http://hkm.cucudq.cn

[R41] 丢弃输出
来源：http://hms.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://gld.zhongyouzk.top

[R42] 输入重定向
来源：http://xsl.xinyue.icu

wc -l < a.txt
来源：http://jgv.shuidangran.top

[R43] 按名字查找文件
来源：http://eom.yanxiufei.cn

find . -name "*.log" -type f
来源：http://fto.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://qfw.daria6918.cn

find . -mtime -7 -type f
来源：http://yhj.gogol.net.cn

[R45] 批量删除
来源：http://tkb.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://zgr.yuxming.cn

[R46] 递归替换文件内容
来源：http://ppj.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mni.fzhhl.top

[R47] sed 单行替换
来源：http://pfu.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://sqf.zhengqikj.top

[R48] awk 取指定列
来源：http://mmx.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://mvk.nanxuanxn.top

[R49] awk 带条件
来源：http://gtw.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ris.yuanzhike.top

[R50] awk 求和
来源：http://xkv.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rge.ybcxt.top

[R51] 排序去重取前几
来源：http://htm.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zgk.quarkkingdee.top

[R52] 统计行数
来源：http://sso.yfazqb.com

wc -l a.txt
来源：http://keb.ivvv.top

[R53] 查看文件头与实时尾
来源：http://erw.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bsj.sysykeji.top

[R54] 比较两个文件
来源：http://mnu.jianghu66.top

diff a.txt b.txt
来源：http://bbv.sxryk.cn

[R55] 压缩与解压
来源：http://ptd.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jua.ehwqpu.com

[R56] 远程拷贝
来源：http://dhh.yonumen.top

scp file user@host:/path/
来源：http://mve.bbcook.cn

[R57] 远程执行命令
来源：http://osk.ydjk.org.cn


<!-- 参考信息 -->