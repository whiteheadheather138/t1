代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yof.sjlbkw.cn

[Q11] 一次插入多行
来源：http://wdi.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hwm.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://foa.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dde.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pov.yj202588.top

[Q13] 忽略重复插入
来源：http://zyy.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rwr.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://rih.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kll.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://thk.haohaochexian.top

[Q15] 查询全部
来源：http://exv.redwolf501.top

SELECT * FROM users;
来源：http://bfh.jlsjyb.cn

[Q16] 查询指定列
来源：http://jth.cucudq.cn

SELECT id, name FROM users;
来源：http://vsw.9152youxi.cn

[Q17] 条件查询
来源：http://oct.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hwr.aibaodan.cn

[Q18] 模糊匹配
来源：http://rzg.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mqi.svipenyu.cn

[Q19] 范围查询
来源：http://rhx.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://glz.yueranfly.top

[Q20] IN 列表
来源：http://rqh.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xyc.316326.xyz

[Q21] 空值判断
来源：http://ije.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://sie.zhaomingkeji.xyz

[Q22] 排序
来源：http://vyc.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uge.bjfxy.top

[Q23] 分页
来源：http://qob.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dqw.yfazqb.com

[Q24] 去重
来源：http://diu.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://jag.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://gcq.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zlz.ywan-chungtsiang.top

[Q26] 计数
来源：http://qvf.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://bef.ehwqpu.com

[Q27] 条件计数
来源：http://xzs.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qpm.yongpay.top

[Q28] 求和与平均
来源：http://hiq.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eza.chenlongwang.top

[Q29] 最大最小值
来源：http://szk.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dey.sjlbkw.cn

[Q30] 分组统计
来源：http://exx.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://weq.guannengcc.top

[Q31] 分组后过滤
来源：http://akj.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aht.yvedp.cn

[Q32] 分组拼接字符串
来源：http://lgu.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iza.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyc.yj20258.top

[Q33] 多列分组
来源：http://uch.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gvk.sufxvd.cn

[Q34] 每组取第一条
来源：http://vsv.daxiang520.top

SELECT * FROM (
来源：http://jfr.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iki.aizwys.cn

) t WHERE rn = 1;
来源：http://aog.yvedp.cn

[Q35] 内连接
来源：http://ciz.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ngv.yj202588.top

[Q36] 左连接
来源：http://ujr.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sfc.yangfankeji.com

[Q37] 右连接
来源：http://zws.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rqb.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zca.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xtl.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://cso.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://oec.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fjs.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jib.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xed.jqgufenzy.top

[Q41] 多表连接
来源：http://ojp.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rrf.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://owk.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mja.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://fep.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://jtx.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gop.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://rmj.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jbx.316326.xyz

[Q44] IN 子查询
来源：http://ube.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwm.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://ywd.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anr.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jqb.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agb.andypj.xyz

[Q47] 与平均值比较
来源：http://ion.haohaochexian.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bro.cheryme.top

[Q48] CTE 公用表表达式
来源：http://lwi.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zyb.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://rkb.daxiang520.top

[Q49] 更新单行
来源：http://rpx.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jek.c1oappe.top

[Q50] 批量更新
来源：http://idi.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lnn.shzxlz.cn

[Q51] 用子查询更新
来源：http://vrw.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gea.wangdashe.top

[Q52] 删除指定行
来源：http://ane.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://ocu.vqdsnc.cn

[Q53] 按条件删除
来源：http://dqm.nanxuanxn.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pec.bjfxy.top

[Q54] 清空表
来源：http://lmf.daria6918.cn

TRUNCATE TABLE logs;
来源：http://wnb.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://uvs.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eux.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://zly.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mqf.dashuyun.cn

[Q57] 行号
来源：http://ntk.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ipq.jqgufenzy.top

[Q58] 累计求和
来源：http://zsq.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wct.haohaochexian.top

[Q59] 分组内累计
来源：http://tjq.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vpk.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://hrs.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vsb.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ite.jqgfzy.top

[Q61] 移动平均
来源：http://pka.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lat.vehdjk.com

[Q62] 分组占比
来源：http://fba.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oku.shanyushiyangtech.top

[Q63] 开启事务
来源：http://apx.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gax.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://ozm.chenjidiqi.icu

COMMIT;
来源：http://nik.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://mgc.pengpengdd.cyou

ROLLBACK;
来源：http://epy.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://mts.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kpt.ivvv.top

[Q67] 设置隔离级别
来源：http://fof.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xwq.hysaishi.cn

[Q68] 保存点
来源：http://apu.epnwcf.com

SAVEPOINT sp1;
来源：http://sor.guannengcc.top

ROLLBACK TO sp1;
来源：http://tek.ydjk.org.cn

[Q69] 查看执行计划
来源：http://esx.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lnr.hywenlv.cn

[Q70] 更新统计信息
来源：http://oxk.zhijiandao.cn

ANALYZE TABLE users;
来源：http://zjd.zhoulong.xyz

[Q71] 查看建表语句
来源：http://kvw.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eid.zdqjudy.top

[Q72] 查看索引
来源：http://ulx.yj202588.top

SHOW INDEX FROM users;
来源：http://als.hysaishi.cn

[Q73] 查看表状态
来源：http://igy.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rxr.yfazqb.com

[Q74] 强制使用索引
来源：http://axs.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gbj.nanxuanxn.top

[Q75] 日期格式化
来源：http://oma.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eqv.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lsv.pengpengdd.cyou

[Q76] 按天统计
来源：http://iyl.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ibx.sufxvd.cn

[Q77] 时间加减
来源：http://yue.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nae.ivvv.top

[Q78] 当前时间
来源：http://yni.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://grf.sweek.top

[Q79] 字符串拼接
来源：http://gxi.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zlc.sjlbkw.cn

[Q80] 字符串截取
来源：http://ysy.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ayg.jiagoushi.top

[Q81] 字符串替换
来源：http://awj.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uzd.meibo888.top

[Q82] 字符长度与字节长度
来源：http://jkq.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wwa.aizwys.cn

[Q83] 大小写转换
来源：http://ykp.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://egj.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://jpn.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://ytx.yueranfly.top

[Q85] 数值取整
来源：http://lrq.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oti.yj202588.top

[Q86] 读取 JSON 字段
来源：http://jmd.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://osh.hesvh.cn

[Q87] JSON 字段做条件
来源：http://gqn.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://buq.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://pln.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kwc.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kxz.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://ren.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gcx.vqdsnc.cn

[Q90] 生成序号列
来源：http://lre.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pyw.gotoacloud.top

================================================================================
来源：http://kmm.guannengcc.top

R. Bash 专题
来源：http://kch.ppjwa.cn

================================================================================
来源：http://zmz.jqgfzy.top

[R01] shebang 与严格模式
来源：http://xvu.bjfxy.top

#!/usr/bin/env bash
来源：http://caz.meibo888.top

set -euo pipefail
来源：http://wwq.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://bcv.fehbvm.com

name="Tom"; echo "$name"
来源：http://daq.epnwcf.com

[R03] 只读变量
来源：http://fpf.gaohongyu789.top

readonly PI=3.14
来源：http://kvj.chenzaomai.com

[R04] 位置参数
来源：http://scs.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cit.kuanghao11.cn

[R05] 参数默认值
来源：http://uqw.zhongyouzk.top

name="${1:-default}"
来源：http://omc.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://gin.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wtn.yvedp.cn

[R07] if 判断文件
来源：http://ayo.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jpl.hcnkem.com

[R08] 数值比较
来源：http://bug.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://khn.xuanzx.com

[R09] 字符串比较
来源：http://pea.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gpw.shangyingyoupin.top

[R10] 正则匹配
来源：http://rlm.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xuo.hysaishi.cn

[R11] case 多分支
来源：http://itf.chenlongwang.top

case "$1" in
来源：http://qnk.ybcxt.top

start) echo "启动" ;;
来源：http://cgb.redwolf501.top

stop)  echo "停止" ;;
来源：http://cxh.fehbvm.com

*)     echo "未知命令" ;;
来源：http://fsg.bjfxy.top

esac
来源：http://skg.epnwcf.com

[R12] for 遍历文件
来源：http://jdo.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://wum.ybcxt.top

[R13] for 计数循环
来源：http://atw.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://unl.fengsongda.top

[R14] C 风格 for
来源：http://qwf.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tov.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://ogg.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxb.shzxlz.cn

[R16] until 等待条件
来源：http://zii.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cdf.hcnkem.com

[R17] 数组定义与取值
来源：http://xsw.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://sjh.tianlin.xyz

[R18] 遍历数组
来源：http://rek.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gis.gotoacloud.top

[R19] 数组长度
来源：http://cir.tarul.cn

echo "${#arr[@]}"
来源：http://bst.pycfn.com

[R20] 关联数组（字典）
来源：http://nin.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aid.tanke756.top

[R21] 字符串长度
来源：http://lkk.zdbjq.cn

echo "${#s}"
来源：http://jcy.yj20258.top

[R22] 截取子串
来源：http://cqo.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://svm.svipenyu.cn

[R23] 字符串替换
来源：http://nxp.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://krl.xuanzx.com

[R24] 大小写转换
来源：http://nsi.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://chs.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://lrp.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bns.fanxiaobao.xyz

[R26] 命令替换
来源：http://eqy.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://van.guowangkeji.top

[R27] 算术展开
来源：http://jdo.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://ara.uphjek.com

[R28] 浮点运算
来源：http://vjp.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://fil.ivvv.top

[R29] 定义函数
来源：http://kvj.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djb.c1oappe.top

[R30] 函数返回状态码
来源：http://zou.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://gwz.meibo888.top

[R31] 局部变量
来源：http://jfd.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://hjl.yonumen.top

[R32] 参数个数校验
来源：http://yqr.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eap.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://unt.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ipo.zhijiandao.cn

[R34] 退出时清理
来源：http://hia.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://cfq.yanxiufei.cn

[R35] 后台执行并等待
来源：http://ryj.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ifz.jinqigufen.top

[R36] 并发执行多个任务
来源：http://ymy.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jcw.redwolf501.top

[R37] 把输出赋给变量
来源：http://iyj.nanxinkj.top

files=$(ls -1)
来源：http://fxn.ydjk.org.cn

[R38] 管道串联
来源：http://vkn.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://vqk.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://rdr.yanxiufei.cn

cmd > out.log 2>&1
来源：http://bkk.feifeiyinyue.top

[R40] 追加写日志
来源：http://uak.zhongyouzk.top

echo "log" >> out.log
来源：http://zgm.hywenlv.cn

[R41] 丢弃输出
来源：http://uqo.bbcook.cn

cmd >/dev/null 2>&1
来源：http://ogr.wangshuangyany.cn

[R42] 输入重定向
来源：http://shc.birdmap.top

wc -l < a.txt
来源：http://uwt.iojbl.cn

[R43] 按名字查找文件
来源：http://fac.svipenyu.cn

find . -name "*.log" -type f
来源：http://vdr.yongpay.top

[R44] 按修改时间查找
来源：http://rhg.fzhhl.top

find . -mtime -7 -type f
来源：http://twf.fzhhl.top

[R45] 批量删除
来源：http://efu.xylfe.cn

find . -name "*.tmp" -delete
来源：http://ukw.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://doh.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hah.chenlongwang.top

[R47] sed 单行替换
来源：http://uss.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://ytc.shangyingyoupin.top

[R48] awk 取指定列
来源：http://mxb.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://bkv.pycfn.com

[R49] awk 带条件
来源：http://fug.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xuu.andypj.xyz

[R50] awk 求和
来源：http://cut.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kiq.aizwys.cn

[R51] 排序去重取前几
来源：http://hqs.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zop.zhijiandao.cn

[R52] 统计行数
来源：http://afa.andypj.xyz

wc -l a.txt
来源：http://pzm.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://uhj.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tqw.ydzc1.top

[R54] 比较两个文件
来源：http://kmb.hongshengwenyu.top

diff a.txt b.txt
来源：http://qxh.52xcode.cn

[R55] 压缩与解压
来源：http://tdf.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yni.cheryme.top

[R56] 远程拷贝
来源：http://jwq.zdqjudy.top

scp file user@host:/path/
来源：http://fnw.sxryk.cn

[R57] 远程执行命令
来源：http://ums.daxiang520.top

ssh user@host 'uptime'
来源：http://fbk.daria6918.cn

[R58] 下载文件
来源：http://mvo.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yyp.sweek.top

[R59] 发 POST JSON
来源：http://isl.cheryme.top


<!-- 参考信息 -->