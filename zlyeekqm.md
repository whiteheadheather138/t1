代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xkb.aizwys.cn

[Q20] IN 列表
来源：http://ckj.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oli.sysykeji.top

[Q21] 空值判断
来源：http://kvr.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iyc.dashuyun.cn

[Q22] 排序
来源：http://hsi.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ozw.hywenlv.cn

[Q23] 分页
来源：http://vld.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ivv.316326.xyz

[Q24] 去重
来源：http://ier.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://gba.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://iol.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tot.fengsongda.top

[Q26] 计数
来源：http://ans.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://tjj.yj202588.top

[Q27] 条件计数
来源：http://bbo.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xfc.uphjek.com

[Q28] 求和与平均
来源：http://rra.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rqu.yj20258.top

[Q29] 最大最小值
来源：http://njz.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://prv.svipenyu.cn

[Q30] 分组统计
来源：http://lqc.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rzl.fzhhl.top

[Q31] 分组后过滤
来源：http://brt.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fbq.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://led.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fou.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qtr.cucudq.cn

[Q33] 多列分组
来源：http://zdb.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fvm.nanxinkj.top

[Q34] 每组取第一条
来源：http://esk.gaohongyu789.top

SELECT * FROM (
来源：http://pov.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kyg.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://sxx.vehdjk.com

[Q35] 内连接
来源：http://nwz.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssv.xinyue.icu

[Q36] 左连接
来源：http://nsh.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ycd.nanxinkj.top

[Q37] 右连接
来源：http://zjz.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uqm.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sld.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ono.birdmap.top

[Q39] 自连接（查上下级）
来源：http://kpu.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://loa.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qqw.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bvu.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nzh.yuxming.cn

[Q41] 多表连接
来源：http://xyv.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wme.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://sxy.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://faf.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://snm.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://zjf.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zby.gotoacloud.top

[Q43] 标量子查询
来源：http://snr.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iii.meibo888.top

[Q44] IN 子查询
来源：http://uqq.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gfu.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://pne.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsc.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://yew.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akf.andypj.xyz

[Q47] 与平均值比较
来源：http://pyk.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hqy.pycfn.com

[Q48] CTE 公用表表达式
来源：http://yrg.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xkw.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://izm.zdbjq.cn

[Q49] 更新单行
来源：http://hlw.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uda.ydjk.org.cn

[Q50] 批量更新
来源：http://mqa.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tsq.jqgufenzy.top

[Q51] 用子查询更新
来源：http://ygf.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ydh.yonumen.top

[Q52] 删除指定行
来源：http://wqh.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://tzc.hysaishi.cn

[Q53] 按条件删除
来源：http://ttb.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://unz.shzxlz.cn

[Q54] 清空表
来源：http://soe.hesvh.cn

TRUNCATE TABLE logs;
来源：http://wzs.havefunace.top

[Q55] 排名（并列占位）
来源：http://kzh.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xbu.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://qer.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://neo.dashuyun.cn

[Q57] 行号
来源：http://zil.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fei.quarkkingdee.top

[Q58] 累计求和
来源：http://lxh.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vca.pengpengdd.cyou

[Q59] 分组内累计
来源：http://tyy.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cip.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://emu.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwb.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ttw.ydjk.org.cn

[Q61] 移动平均
来源：http://yuo.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cov.zhixingplan.top

[Q62] 分组占比
来源：http://acg.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://phm.zhongyouzk.top

[Q63] 开启事务
来源：http://iya.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lqr.fzhhl.top

[Q64] 提交事务
来源：http://ppb.snrcjt.cn

COMMIT;
来源：http://fvn.cucudq.cn

[Q65] 回滚事务
来源：http://vmf.zycfv.cn

ROLLBACK;
来源：http://kfq.fktsv.cn

[Q66] 行锁查询
来源：http://zab.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sjt.zhixingplan.top

[Q67] 设置隔离级别
来源：http://izw.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xkg.epnwcf.com

[Q68] 保存点
来源：http://kgw.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://yae.meibo888.top

ROLLBACK TO sp1;
来源：http://nzk.tanke756.top

[Q69] 查看执行计划
来源：http://yze.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axm.hnxiangtu.top

[Q70] 更新统计信息
来源：http://wpv.nwbrower.top

ANALYZE TABLE users;
来源：http://nwh.iojbl.cn

[Q71] 查看建表语句
来源：http://uxd.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ztx.andypj.xyz

[Q72] 查看索引
来源：http://zeq.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://our.ehwqpu.com

[Q73] 查看表状态
来源：http://beh.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zhd.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://wbs.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tlr.xylfe.cn

[Q75] 日期格式化
来源：http://xzh.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pzx.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://azu.9152youxi.cn

[Q76] 按天统计
来源：http://ccp.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://olk.ctjpmb.com

[Q77] 时间加减
来源：http://vwb.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jxs.aibaodan.cn

[Q78] 当前时间
来源：http://hif.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://egt.uphjek.com

[Q79] 字符串拼接
来源：http://jvh.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nop.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://wdg.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://syb.havefunace.top

[Q81] 字符串替换
来源：http://leg.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jtm.cheryme.top

[Q82] 字符长度与字节长度
来源：http://rme.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bdu.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://mlx.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aei.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://qvo.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://ums.wangshuangyany.cn

[Q85] 数值取整
来源：http://ghh.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mbl.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://okr.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wnj.daxiang520.top

[Q87] JSON 字段做条件
来源：http://upi.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://spr.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://jzd.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzt.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xst.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://pvu.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sbi.yongpay.top

[Q90] 生成序号列
来源：http://nws.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rqw.52xcode.cn

================================================================================
来源：http://kfq.cashguo.top

R. Bash 专题
来源：http://vkw.xuetiantiany.cn

================================================================================
来源：http://hcv.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://ahk.pycfn.com

#!/usr/bin/env bash
来源：http://pko.quarkkingdee.top

set -euo pipefail
来源：http://mmo.fzhhl.top

[R02] 变量赋值与使用
来源：http://ene.daxiang520.top

name="Tom"; echo "$name"
来源：http://dgd.yonumen.top

[R03] 只读变量
来源：http://wln.jyoumei.cn

readonly PI=3.14
来源：http://ccy.pengpengdd.cyou

[R04] 位置参数
来源：http://gcl.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtq.hfpthk.cn

[R05] 参数默认值
来源：http://cir.zhaomingkeji.xyz

name="${1:-default}"
来源：http://rpm.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://skk.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hlf.zdqjudy.top

[R07] if 判断文件
来源：http://tlv.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sjh.nanxuanxn.top

[R08] 数值比较
来源：http://myv.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ktv.svipenyu.cn

[R09] 字符串比较
来源：http://lpm.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aqu.nanxinkj.top

[R10] 正则匹配
来源：http://zml.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xni.zhijiandao.cn

[R11] case 多分支
来源：http://opu.pengpengdd.cyou

case "$1" in
来源：http://wzh.fzhhl.top

start) echo "启动" ;;
来源：http://yxg.jinqigufen.top

stop)  echo "停止" ;;
来源：http://mlv.guannengcc.top

*)     echo "未知命令" ;;
来源：http://ioh.hnxiangtu.top

esac
来源：http://dmw.zhengqikj.top

[R12] for 遍历文件
来源：http://mcn.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://vgu.xylfe.cn

[R13] for 计数循环
来源：http://lic.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://nea.hammf.cn

[R14] C 风格 for
来源：http://xtg.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://emd.bjfxy.top

[R15] while 逐行读文件
来源：http://onk.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vkg.gaohongyu789.top

[R16] until 等待条件
来源：http://wvc.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwa.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://axj.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://jho.cdnleiting.top

[R18] 遍历数组
来源：http://yct.jqgfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vjh.svipenyu.cn

[R19] 数组长度
来源：http://wty.wangdashe.top

echo "${#arr[@]}"
来源：http://loh.sysykeji.top

[R20] 关联数组（字典）
来源：http://iha.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://don.chenlongwang.top

[R21] 字符串长度
来源：http://fzv.snrcjt.cn

echo "${#s}"
来源：http://czy.jqgufenzy.top

[R22] 截取子串
来源：http://bcy.hongshengwenyu.top

echo "${s:0:5}"
来源：http://twd.gaohongyu789.top

[R23] 字符串替换
来源：http://upv.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tua.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://gqy.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qdr.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://yfa.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ozz.daxiang520.top

[R26] 命令替换
来源：http://ray.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://coy.aibaodan.cn

[R27] 算术展开
来源：http://egg.shuidangran.top

echo $((1 + 2 * 3))
来源：http://lml.andypj.xyz

[R28] 浮点运算
来源：http://poz.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://jky.hysaishi.cn

[R29] 定义函数
来源：http://xgy.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gbj.bjfxy.top

[R30] 函数返回状态码
来源：http://lbv.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://tzd.aizwys.cn

[R31] 局部变量
来源：http://wlw.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://jiu.sufxvd.cn

[R32] 参数个数校验
来源：http://ygf.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tjb.sweek.top

[R33] 捕获错误并提示行号
来源：http://dqy.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rwp.quarkkingdee.top

[R34] 退出时清理
来源：http://pkn.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ajs.tanke756.top

[R35] 后台执行并等待
来源：http://fpk.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ldh.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://brd.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dyh.zhengqikj.top

[R37] 把输出赋给变量
来源：http://tgq.zdqjudy.top

files=$(ls -1)
来源：http://fri.havefunace.top

[R38] 管道串联
来源：http://ale.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://fxk.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://kcu.hnqzz.top

cmd > out.log 2>&1
来源：http://wmh.yvedp.cn

[R40] 追加写日志
来源：http://duu.vqdsnc.cn

echo "log" >> out.log
来源：http://lps.cucudq.cn

[R41] 丢弃输出
来源：http://ibb.52xcode.cn

cmd >/dev/null 2>&1
来源：http://fgs.jiagoushi.top

[R42] 输入重定向
来源：http://nco.zhongyouzk.top

wc -l < a.txt
来源：http://kcj.vqdsnc.cn

[R43] 按名字查找文件
来源：http://whg.hywenlv.cn

find . -name "*.log" -type f
来源：http://ued.hcnkem.com

[R44] 按修改时间查找
来源：http://nuq.yj20258.top

find . -mtime -7 -type f
来源：http://tnq.jlsjyb.cn

[R45] 批量删除
来源：http://xex.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://ytl.ehwqpu.com

[R46] 递归替换文件内容
来源：http://jzb.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sfm.gogol.net.cn

[R47] sed 单行替换
来源：http://dpd.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oss.jiagoushi.top

[R48] awk 取指定列
来源：http://btb.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://gyo.nanxuanxn.top

[R49] awk 带条件
来源：http://mpi.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qik.guowangkeji.top

[R50] awk 求和
来源：http://hbb.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://mhc.nwbrower.top

[R51] 排序去重取前几
来源：http://obs.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://epn.redwolf501.top

[R52] 统计行数
来源：http://jbv.chenjidiqi.icu

wc -l a.txt
来源：http://rjk.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://aob.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lpz.xuanzx.com

[R54] 比较两个文件
来源：http://idk.meibo888.top

diff a.txt b.txt
来源：http://piq.52xcode.cn

[R55] 压缩与解压
来源：http://veq.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fyu.jlsjyb.cn

[R56] 远程拷贝
来源：http://wqz.xuetiantiany.cn

scp file user@host:/path/
来源：http://ptt.yuxming.cn

[R57] 远程执行命令
来源：http://tdw.fktsv.cn

ssh user@host 'uptime'
来源：http://fgp.gzhubu.top

[R58] 下载文件
来源：http://okp.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tay.cheryme.top

[R59] 发 POST JSON
来源：http://yds.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fgj.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://aet.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fxa.xinyue.icu

[R61] 磁盘占用
来源：http://jul.quarkkingdee.top

df -h;  du -sh *
来源：http://yul.pycfn.com

[R62] 找最占空间的文件
来源：http://lnd.316326.xyz

du -ah . | sort -rh | head -10
来源：http://foc.chenlongwang.top

[R63] 内存与进程
来源：http://bjd.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://ius.yj202588.top

[R64] 结束进程
来源：http://dwt.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://azo.fengsongda.top

[R65] 查看端口占用
来源：http://tim.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dma.jianghu66.top

[R66] 定时任务
来源：http://xns.kuanghao11.cn

crontab -e;  crontab -l
来源：http://gnj.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://boa.ehwqpu.com

openssl rand -hex 16
来源：http://lmu.ehwqpu.com

[R68] 计算文件校验值
来源：http://pxa.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://osb.hnqzz.top

[R69] 生成随机密码
来源：http://mmy.dashuyun.cn


<!-- 参考信息 -->