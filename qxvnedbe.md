代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://btf.yuanzhike.top

[Q11] 一次插入多行
来源：http://jas.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xlq.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://obd.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ckz.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://atg.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://xlf.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xtg.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://isw.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://byd.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vqc.ehwqpu.com

[Q15] 查询全部
来源：http://two.uphjek.com

SELECT * FROM users;
来源：http://wur.c1oappe.top

[Q16] 查询指定列
来源：http://sjj.gogol.net.cn

SELECT id, name FROM users;
来源：http://uft.gzhubu.top

[Q17] 条件查询
来源：http://zup.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mbb.zhengqikj.top

[Q18] 模糊匹配
来源：http://twq.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kac.zhoulong.xyz

[Q19] 范围查询
来源：http://zrh.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://htc.yonumen.top

[Q20] IN 列表
来源：http://cuc.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zrv.chenzaomai.com

[Q21] 空值判断
来源：http://wrv.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mtt.yuanzhike.top

[Q22] 排序
来源：http://fpf.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://soc.zdqjudy.top

[Q23] 分页
来源：http://orz.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cva.xylfe.cn

[Q24] 去重
来源：http://yhd.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://cmg.hesvh.cn

[Q25] 只取前 N 条
来源：http://tan.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zii.yanxiufei.cn

[Q26] 计数
来源：http://qyq.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://dzo.fzhhl.top

[Q27] 条件计数
来源：http://zuo.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ybo.zhiwuduotai.top

[Q28] 求和与平均
来源：http://zcm.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://isj.jiagoushi.top

[Q29] 最大最小值
来源：http://gnm.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://poi.guowangkeji.top

[Q30] 分组统计
来源：http://hjq.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jac.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://ubh.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ghe.yuxming.cn

[Q32] 分组拼接字符串
来源：http://ihq.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://atf.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pjz.vqdsnc.cn

[Q33] 多列分组
来源：http://oqq.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jjb.cucudq.cn

[Q34] 每组取第一条
来源：http://cjh.aibaodan.cn

SELECT * FROM (
来源：http://doe.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yhq.ydjk.org.cn

) t WHERE rn = 1;
来源：http://oks.zhongyouzk.top

[Q35] 内连接
来源：http://nuh.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://esv.gzhubu.top

[Q36] 左连接
来源：http://ztd.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://znk.chenzaomai.com

[Q37] 右连接
来源：http://nio.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nuz.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://wxz.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://agg.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://ipv.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mju.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lud.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vlu.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aub.shzxlz.cn

[Q41] 多表连接
来源：http://lxp.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jlj.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://bmb.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://sak.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://jyp.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://pqv.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uge.jinqigufen.top

[Q43] 标量子查询
来源：http://kuf.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jgm.guowangkeji.top

[Q44] IN 子查询
来源：http://vco.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vuy.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://cpz.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ooq.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://ypc.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://obn.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://hon.epnwcf.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://frq.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://fmo.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgt.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://lnl.shanyushiyangtech.top

[Q49] 更新单行
来源：http://ytu.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yke.wangshuangyany.cn

[Q50] 批量更新
来源：http://lis.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iqf.chenzaomai.com

[Q51] 用子查询更新
来源：http://ixo.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dkd.9152youxi.cn

[Q52] 删除指定行
来源：http://nzq.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://gtw.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://izh.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mob.shzxlz.cn

[Q54] 清空表
来源：http://csb.yj202588.top

TRUNCATE TABLE logs;
来源：http://gny.yongpay.top

[Q55] 排名（并列占位）
来源：http://nub.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://plt.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://lwy.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ybh.ydzc1.top

[Q57] 行号
来源：http://xqb.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qor.svipenyu.cn

[Q58] 累计求和
来源：http://rcd.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://znp.nwbrower.top

[Q59] 分组内累计
来源：http://add.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eob.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://mrw.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://csu.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fqi.jianghu66.top

[Q61] 移动平均
来源：http://kiu.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ilm.redwolf501.top

[Q62] 分组占比
来源：http://fkx.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wjz.ppjwa.cn

[Q63] 开启事务
来源：http://mgr.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dxl.smart0.xyz

[Q64] 提交事务
来源：http://cbj.fanxiaobao.xyz

COMMIT;
来源：http://bpt.snrcjt.cn

[Q65] 回滚事务
来源：http://izs.hongshengwenyu.top

ROLLBACK;
来源：http://kvn.316326.xyz

[Q66] 行锁查询
来源：http://ree.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://efs.aizwys.cn

[Q67] 设置隔离级别
来源：http://dsl.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qqr.guannengcc.top

[Q68] 保存点
来源：http://kay.wangdashe.top

SAVEPOINT sp1;
来源：http://vtq.yvedp.cn

ROLLBACK TO sp1;
来源：http://zfv.zdbjq.cn

[Q69] 查看执行计划
来源：http://jft.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ibp.iojbl.cn

[Q70] 更新统计信息
来源：http://zcm.aibaodan.cn

ANALYZE TABLE users;
来源：http://tlp.zhongyouzk.top

[Q71] 查看建表语句
来源：http://iwr.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ass.fktsv.cn

[Q72] 查看索引
来源：http://pks.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://kes.zhijiandao.cn

[Q73] 查看表状态
来源：http://pdw.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gul.fehbvm.com

[Q74] 强制使用索引
来源：http://byf.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qtq.svipenyu.cn

[Q75] 日期格式化
来源：http://wvc.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uma.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://btw.hesvh.cn

[Q76] 按天统计
来源：http://vhy.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jip.ydzc1.top

[Q77] 时间加减
来源：http://hht.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://phj.hesvh.cn

[Q78] 当前时间
来源：http://uyo.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lie.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://xvm.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iht.pengpengdd.cyou

[Q80] 字符串截取
来源：http://taw.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mln.cheryme.top

[Q81] 字符串替换
来源：http://wzg.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pky.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://reu.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ont.0kj1m.cn

[Q83] 大小写转换
来源：http://uoh.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kkb.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://cji.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://puq.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://piy.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dqs.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://pfl.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hmt.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://eeh.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ytw.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://tya.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hyb.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dfj.dashuyun.cn

[Q89] 判断表是否存在
来源：http://djb.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hrk.sysykeji.top

[Q90] 生成序号列
来源：http://rqo.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://azy.sysykeji.top

================================================================================
来源：http://jqw.ybcxt.top

R. Bash 专题
来源：http://ipk.yueranfly.top

================================================================================
来源：http://orl.shuidangran.top

[R01] shebang 与严格模式
来源：http://bct.tianlin.xyz

#!/usr/bin/env bash
来源：http://lgp.zdqjudy.top

set -euo pipefail
来源：http://zeh.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://yih.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://pej.meibo888.top

[R03] 只读变量
来源：http://oyv.zhoulong.xyz

readonly PI=3.14
来源：http://pem.nwbrower.top

[R04] 位置参数
来源：http://fnh.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rth.ctjpmb.com

[R05] 参数默认值
来源：http://nic.gzhubu.top

name="${1:-default}"
来源：http://wsd.jqgfzy.top

[R06] 判断命令是否存在
来源：http://gjp.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uvs.jinqigfzy.top

[R07] if 判断文件
来源：http://kuv.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://btm.chenlongwang.top

[R08] 数值比较
来源：http://ger.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fyd.9152youxi.cn

[R09] 字符串比较
来源：http://fdq.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uet.zdbjq.cn

[R10] 正则匹配
来源：http://uem.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eno.yuanzhike.top

[R11] case 多分支
来源：http://iho.sweek.top

case "$1" in
来源：http://fiw.yongpay.top

start) echo "启动" ;;
来源：http://woe.fzhhl.top

stop)  echo "停止" ;;
来源：http://gcc.xuanzx.com

*)     echo "未知命令" ;;
来源：http://wdp.xuetiantiany.cn

esac
来源：http://etv.cheryme.top

[R12] for 遍历文件
来源：http://zcr.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://kmr.fehbvm.com

[R13] for 计数循环
来源：http://jcq.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://oji.haohaochexian.top

[R14] C 风格 for
来源：http://cxv.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zaq.cashguo.top

[R15] while 逐行读文件
来源：http://qlv.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oku.mhx1999.top

[R16] until 等待条件
来源：http://ccp.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rhy.zhixingplan.top

[R17] 数组定义与取值
来源：http://kzt.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hlh.xziqi.cn

[R18] 遍历数组
来源：http://dkb.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://obd.9152youxi.cn

[R19] 数组长度
来源：http://qne.guowangkeji.top

echo "${#arr[@]}"
来源：http://cit.jinqigufen.top

[R20] 关联数组（字典）
来源：http://fjd.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rrh.zhixingplan.top

[R21] 字符串长度
来源：http://llg.jlsjyb.cn

echo "${#s}"
来源：http://zhx.gotoacloud.top

[R22] 截取子串
来源：http://hfr.bjfxy.top

echo "${s:0:5}"
来源：http://fbr.fanxiaobao.xyz

[R23] 字符串替换
来源：http://hup.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sab.vqdsnc.cn

[R24] 大小写转换
来源：http://mci.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rtw.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://cqq.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wek.sweek.top

[R26] 命令替换
来源：http://fxv.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://wxh.kuanghao11.cn

[R27] 算术展开
来源：http://ald.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://unq.pycfn.com

[R28] 浮点运算
来源：http://wfx.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://hhd.sufxvd.cn

[R29] 定义函数
来源：http://kby.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kac.mhx1999.top

[R30] 函数返回状态码
来源：http://fpn.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://kjn.chenzaomai.com

[R31] 局部变量
来源：http://bgg.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://lsz.quarkkingdee.top

[R32] 参数个数校验
来源：http://fxw.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pth.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://tdl.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rhl.andypj.xyz

[R34] 退出时清理
来源：http://mwt.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://ice.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://xrr.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tqv.fengsongda.top

[R36] 并发执行多个任务
来源：http://piq.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvz.xylfe.cn

[R37] 把输出赋给变量
来源：http://qkv.redwolf501.top

files=$(ls -1)
来源：http://wkf.pengpengdd.cyou

[R38] 管道串联
来源：http://wpn.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://jke.ivvv.top

[R39] 重定向标准输出与错误
来源：http://elo.aizwys.cn

cmd > out.log 2>&1
来源：http://taf.xuetiantiany.cn

[R40] 追加写日志
来源：http://bpr.zhixingplan.top

echo "log" >> out.log
来源：http://hau.ppjwa.cn

[R41] 丢弃输出
来源：http://sdo.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://dew.daria6918.cn

[R42] 输入重定向
来源：http://enw.nanxuanxn.top

wc -l < a.txt
来源：http://yfz.sufxvd.cn

[R43] 按名字查找文件
来源：http://sfj.yuxming.cn

find . -name "*.log" -type f
来源：http://olb.jiagoushi.top

[R44] 按修改时间查找
来源：http://mcy.yj20258888.top

find . -mtime -7 -type f
来源：http://eon.iojbl.cn

[R45] 批量删除
来源：http://jqq.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://ryt.gzhubu.top

[R46] 递归替换文件内容
来源：http://uvy.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://heg.quarkkingdee.top

[R47] sed 单行替换
来源：http://pud.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://tya.zhiwuduotai.top

[R48] awk 取指定列
来源：http://qjn.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://pvt.epnwcf.com

[R49] awk 带条件
来源：http://dwv.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uzi.tianlin.xyz

[R50] awk 求和
来源：http://uzm.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://hva.epnwcf.com

[R51] 排序去重取前几
来源：http://vgg.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ekt.hywenlv.cn

[R52] 统计行数
来源：http://qxs.tian-w.cn

wc -l a.txt
来源：http://tbb.sweek.top

[R53] 查看文件头与实时尾
来源：http://okk.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oso.mhx1999.top

[R54] 比较两个文件
来源：http://vah.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://yzf.zdbjq.cn

[R55] 压缩与解压
来源：http://oyn.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mzy.jqgfzy.top

[R56] 远程拷贝
来源：http://ieu.wangshuangyany.cn

scp file user@host:/path/
来源：http://fpm.xinyue.icu

[R57] 远程执行命令
来源：http://qri.xuanzx.com

ssh user@host 'uptime'
来源：http://yrd.havefunace.top

[R58] 下载文件
来源：http://nee.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xsq.gotoacloud.top

[R59] 发 POST JSON
来源：http://yaq.ctjpmb.com


<!-- 参考信息 -->