代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cje.zhongyouzk.top

) t WHERE rn = 1;
来源：http://aum.vehdjk.com

[Q35] 内连接
来源：http://ins.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jqf.hfpthk.cn

[Q36] 左连接
来源：http://aez.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aag.jinyuanbaomall.cn

[Q37] 右连接
来源：http://jzt.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wfc.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qec.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uza.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://vgl.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://atv.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pbu.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pzx.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zvm.svipenyu.cn

[Q41] 多表连接
来源：http://wvh.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ysi.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://yjq.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://hnj.yongpay.top

[Q42] 连接条件附加过滤
来源：http://kks.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://nle.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kim.xuanzx.com

[Q43] 标量子查询
来源：http://lzn.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://thm.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://bpi.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iau.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://lzl.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fyv.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://bzn.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blg.xinyue.icu

[Q47] 与平均值比较
来源：http://fef.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yzi.yj20258.top

[Q48] CTE 公用表表达式
来源：http://gcy.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gqc.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://gmz.jyoumei.cn

[Q49] 更新单行
来源：http://yeb.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cgl.aizwys.cn

[Q50] 批量更新
来源：http://qdd.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zvp.sjlbkw.cn

[Q51] 用子查询更新
来源：http://wuz.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yek.svipenyu.cn

[Q52] 删除指定行
来源：http://lkd.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://ejv.vehdjk.com

[Q53] 按条件删除
来源：http://wjs.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://msm.ppjwa.cn

[Q54] 清空表
来源：http://fyy.fehbvm.com

TRUNCATE TABLE logs;
来源：http://szh.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://bfo.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bsa.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://psa.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hha.yj20258.top

[Q57] 行号
来源：http://xjd.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vqs.pycfn.com

[Q58] 累计求和
来源：http://dhc.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xol.guowangkeji.top

[Q59] 分组内累计
来源：http://fyg.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbt.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://jwg.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hax.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cqp.zhixingplan.top

[Q61] 移动平均
来源：http://bmp.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ctk.daria6918.cn

[Q62] 分组占比
来源：http://cfj.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://owd.fehbvm.com

[Q63] 开启事务
来源：http://wqu.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kis.jiagoushi.top

[Q64] 提交事务
来源：http://enz.tianlin.xyz

COMMIT;
来源：http://oyn.ctjpmb.com

[Q65] 回滚事务
来源：http://bbb.cqqwz.cn

ROLLBACK;
来源：http://bux.tanke756.top

[Q66] 行锁查询
来源：http://wqf.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hej.redwolf501.top

[Q67] 设置隔离级别
来源：http://wod.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lvd.hysaishi.cn

[Q68] 保存点
来源：http://ntk.sxryk.cn

SAVEPOINT sp1;
来源：http://ynh.daxiang520.top

ROLLBACK TO sp1;
来源：http://tvf.fzhhl.top

[Q69] 查看执行计划
来源：http://mxb.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uax.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://wpx.gzhubu.top

ANALYZE TABLE users;
来源：http://knx.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://nyo.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wmm.yangfankeji.com

[Q72] 查看索引
来源：http://aky.havefunace.top

SHOW INDEX FROM users;
来源：http://pul.hammf.cn

[Q73] 查看表状态
来源：http://yot.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lnj.gaohongyu789.top

[Q74] 强制使用索引
来源：http://tlv.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mcb.zhoulong.xyz

[Q75] 日期格式化
来源：http://cmp.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xfs.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://msq.xziqi.cn

[Q76] 按天统计
来源：http://cwd.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jys.sxryk.cn

[Q77] 时间加减
来源：http://czw.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://awr.xziqi.cn

[Q78] 当前时间
来源：http://sns.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://isv.cqqwz.cn

[Q79] 字符串拼接
来源：http://xgn.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eim.c1oappe.top

[Q80] 字符串截取
来源：http://xku.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mpb.xinyue.icu

[Q81] 字符串替换
来源：http://kyd.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mpz.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://luu.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nvn.jianghu66.top

[Q83] 大小写转换
来源：http://mop.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pow.hesvh.cn

[Q84] 去除首尾空格
来源：http://oix.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://qje.havefunace.top

[Q85] 数值取整
来源：http://fsp.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rem.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://uoc.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jcr.yfazqb.com

[Q87] JSON 字段做条件
来源：http://pbw.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zmp.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://apr.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://feq.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xoi.redwolf501.top

[Q89] 判断表是否存在
来源：http://bod.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dup.smart0.xyz

[Q90] 生成序号列
来源：http://rzq.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mks.sufxvd.cn

================================================================================
来源：http://zje.fehbvm.com

R. Bash 专题
来源：http://tvj.sxryk.cn

================================================================================
来源：http://xgl.c1oappe.top

[R01] shebang 与严格模式
来源：http://xsa.yonumen.top

#!/usr/bin/env bash
来源：http://fvw.snrcjt.cn

set -euo pipefail
来源：http://dpt.sweek.top

[R02] 变量赋值与使用
来源：http://bpq.zycfv.cn

name="Tom"; echo "$name"
来源：http://zds.cucudq.cn

[R03] 只读变量
来源：http://uca.jinqigufen.top

readonly PI=3.14
来源：http://ggb.mhx1999.top

[R04] 位置参数
来源：http://bon.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gcj.9152youxi.cn

[R05] 参数默认值
来源：http://tzl.yonumen.top

name="${1:-default}"
来源：http://tha.hysaishi.cn

[R06] 判断命令是否存在
来源：http://mhe.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bxd.hongshengwenyu.top

[R07] if 判断文件
来源：http://fnx.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ium.sjlbkw.cn

[R08] 数值比较
来源：http://ppz.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vuv.sysykeji.top

[R09] 字符串比较
来源：http://xen.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qcg.svipenyu.cn

[R10] 正则匹配
来源：http://vde.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zlo.shzxlz.cn

[R11] case 多分支
来源：http://oqb.daxiang520.top

case "$1" in
来源：http://jsp.guowangkeji.top

start) echo "启动" ;;
来源：http://yen.ppjwa.cn

stop)  echo "停止" ;;
来源：http://byq.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://rtl.aizwys.cn

esac
来源：http://qwa.vehdjk.com

[R12] for 遍历文件
来源：http://crr.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://egn.vehdjk.com

[R13] for 计数循环
来源：http://gvu.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://qgx.9152youxi.cn

[R14] C 风格 for
来源：http://kvb.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zni.sweek.top

[R15] while 逐行读文件
来源：http://jib.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mhg.birdmap.top

[R16] until 等待条件
来源：http://jeb.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vqh.yj202588.top

[R17] 数组定义与取值
来源：http://slt.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xkx.sxryk.cn

[R18] 遍历数组
来源：http://hml.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gtk.meibo888.top

[R19] 数组长度
来源：http://iif.jlsjyb.cn

echo "${#arr[@]}"
来源：http://uaa.jyoumei.cn

[R20] 关联数组（字典）
来源：http://rlx.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxc.shanyushiyangtech.top

[R21] 字符串长度
来源：http://wrr.chenzaomai.com

echo "${#s}"
来源：http://uhg.nanxinkj.top

[R22] 截取子串
来源：http://jyu.yongpay.top

echo "${s:0:5}"
来源：http://umd.sufxvd.cn

[R23] 字符串替换
来源：http://cuk.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fqd.xuanzx.com

[R24] 大小写转换
来源：http://viu.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://pcp.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://omj.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dnj.havefunace.top

[R26] 命令替换
来源：http://qes.yj20258.top

now=$(date +%F); echo "$now"
来源：http://jia.shuidangran.top

[R27] 算术展开
来源：http://cdr.ydzc1.top

echo $((1 + 2 * 3))
来源：http://nsa.yj20258.top

[R28] 浮点运算
来源：http://eut.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://mmw.9152youxi.cn

[R29] 定义函数
来源：http://wka.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vvh.gogol.net.cn

[R30] 函数返回状态码
来源：http://fdj.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://mdj.jyoumei.cn

[R31] 局部变量
来源：http://khb.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://irg.316326.xyz

[R32] 参数个数校验
来源：http://air.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ffv.yj20258.top

[R33] 捕获错误并提示行号
来源：http://vox.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://byi.c1oappe.top

[R34] 退出时清理
来源：http://khi.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://fql.zhongyouzk.top

[R35] 后台执行并等待
来源：http://vqy.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cen.yonumen.top

[R36] 并发执行多个任务
来源：http://qxo.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zug.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://ohw.jianghu66.top

files=$(ls -1)
来源：http://ppe.andypj.xyz

[R38] 管道串联
来源：http://otl.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://xua.cashguo.top

[R39] 重定向标准输出与错误
来源：http://qqm.mhx1999.top

cmd > out.log 2>&1
来源：http://otq.bbcook.cn

[R40] 追加写日志
来源：http://dag.snrcjt.cn

echo "log" >> out.log
来源：http://vhs.kuanghao11.cn

[R41] 丢弃输出
来源：http://svm.xylfe.cn

cmd >/dev/null 2>&1
来源：http://vli.yvedp.cn

[R42] 输入重定向
来源：http://ghr.hnqzz.top

wc -l < a.txt
来源：http://mmc.yanxiufei.cn

[R43] 按名字查找文件
来源：http://xld.jyoumei.cn

find . -name "*.log" -type f
来源：http://qym.sysykeji.top

[R44] 按修改时间查找
来源：http://glz.ppjwa.cn

find . -mtime -7 -type f
来源：http://izl.nanxuanxn.top

[R45] 批量删除
来源：http://epp.epnwcf.com

find . -name "*.tmp" -delete
来源：http://jdr.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://qav.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://irl.52xcode.cn

[R47] sed 单行替换
来源：http://pnh.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://tbs.shangyingyoupin.top

[R48] awk 取指定列
来源：http://uty.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://fsl.yj202588.top

[R49] awk 带条件
来源：http://mrr.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://paw.ywan-chungtsiang.top

[R50] awk 求和
来源：http://dje.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wls.yvedp.cn

[R51] 排序去重取前几
来源：http://vmp.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hso.sxryk.cn

[R52] 统计行数
来源：http://ifa.chenlongwang.top

wc -l a.txt
来源：http://yyu.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://mxv.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://loj.xuetiantiany.cn

[R54] 比较两个文件
来源：http://ked.dianchejie.cn

diff a.txt b.txt
来源：http://mid.tian-w.cn

[R55] 压缩与解压
来源：http://szv.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gwp.zdbjq.cn

[R56] 远程拷贝
来源：http://sji.hongshengwenyu.top

scp file user@host:/path/
来源：http://jrx.haohaochexian.top

[R57] 远程执行命令
来源：http://bre.havefunace.top

ssh user@host 'uptime'
来源：http://zvp.nwbrower.top

[R58] 下载文件
来源：http://xku.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aod.xinyue.icu

[R59] 发 POST JSON
来源：http://bus.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zfs.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://pen.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bmi.gogol.net.cn

[R61] 磁盘占用
来源：http://pmc.ehwqpu.com

df -h;  du -sh *
来源：http://kbg.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://iwh.sufxvd.cn

du -ah . | sort -rh | head -10
来源：http://gla.yuanzhike.top

[R63] 内存与进程
来源：http://ncr.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://lho.cashguo.top

[R64] 结束进程
来源：http://ork.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://ozn.sufxvd.cn

[R65] 查看端口占用
来源：http://zqd.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rif.fzhhl.top

[R66] 定时任务
来源：http://yau.ydzc1.top

crontab -e;  crontab -l
来源：http://phf.yj202588.top

[R67] 生成随机十六进制串
来源：http://amq.yj202588.top

openssl rand -hex 16
来源：http://qky.ivvv.top

[R68] 计算文件校验值
来源：http://smx.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://eun.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://efn.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://eea.fzhhl.top

[R70] 时间戳与互转
来源：http://rja.tanke756.top

date +%s;  date -d @1700000000
来源：http://qta.yvedp.cn

[R71] 日期格式化
来源：http://rma.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ygf.sxryk.cn

[R72] 等待端口就绪
来源：http://wue.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://czw.zdqjudy.top

[R73] 分割大日志
来源：http://ttd.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://dhl.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://awq.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zqc.tarul.cn

[R75] 导出环境变量
来源：http://xlo.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://rqa.wangshuangyany.cn

[R76] 使用临时文件
来源：http://jco.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wks.epnwcf.com

[R77] 读取用户输入
来源：http://llp.daxiang520.top

read -rp "请输入: " ans
来源：http://pgs.feifeiyinyue.top

[R78] 交互式菜单
来源：http://gff.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://igm.yj20258.top

[R79] 解析命令行选项
来源：http://lil.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cyc.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://zim.zdbjq.cn

time ./run.sh
来源：http://qse.hywenlv.cn

================================================================================
来源：http://nnd.xylfe.cn

S. C / C++ 专题
来源：http://mqk.tanke756.top

================================================================================
来源：http://hir.sweek.top

[S01] C：Hello World
来源：http://bkk.uphjek.com

#include <stdio.h>
来源：http://nuo.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fwm.hammf.cn

[S02] C：变量与格式化输出
来源：http://zhp.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://nqn.yueranfly.top

[S03] C：读入整数
来源：http://pzg.yuxming.cn


<!-- 参考信息 -->