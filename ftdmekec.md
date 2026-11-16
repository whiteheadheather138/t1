代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ftj.gotoacloud.top

[Q28] 求和与平均
来源：http://tzo.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lra.hywenlv.cn

[Q29] 最大最小值
来源：http://yfs.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://six.redwolf501.top

[Q30] 分组统计
来源：http://wuy.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcj.tian-w.cn

[Q31] 分组后过滤
来源：http://zhu.jinqigfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sod.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://dyv.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xsl.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nrx.cdnleiting.top

[Q33] 多列分组
来源：http://dpw.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qhy.fktsv.cn

[Q34] 每组取第一条
来源：http://tho.hysaishi.cn

SELECT * FROM (
来源：http://rdr.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uqs.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://pep.meibo888.top

[Q35] 内连接
来源：http://yua.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yiq.haohaochexian.top

[Q36] 左连接
来源：http://bfr.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jrp.9152youxi.cn

[Q37] 右连接
来源：http://hvg.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cqk.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mmk.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jqv.sweek.top

[Q39] 自连接（查上下级）
来源：http://czd.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mkg.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iiv.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zwv.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://isg.fengsongda.top

[Q41] 多表连接
来源：http://jzz.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uha.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://mnx.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://kog.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://vvk.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://ftp.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wdj.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://fix.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dwa.quarkkingdee.top

[Q44] IN 子查询
来源：http://gun.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uzb.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://lik.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqf.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://qji.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ygr.wangdashe.top

[Q47] 与平均值比较
来源：http://tap.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://abq.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://xje.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://smi.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://gcm.yueranfly.top

[Q49] 更新单行
来源：http://mjm.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ine.jinqigufen.top

[Q50] 批量更新
来源：http://qma.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rtq.chenzaomai.com

[Q51] 用子查询更新
来源：http://zlo.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wwp.mhx1999.top

[Q52] 删除指定行
来源：http://ovt.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://tvl.zdqjudy.top

[Q53] 按条件删除
来源：http://mgu.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hro.yj202588.top

[Q54] 清空表
来源：http://odj.fktsv.cn

TRUNCATE TABLE logs;
来源：http://bvm.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://rrg.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vpj.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://rpd.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pow.zhaomingkeji.xyz

[Q57] 行号
来源：http://wqb.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dft.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://enl.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uia.zhengqikj.top

[Q59] 分组内累计
来源：http://rkz.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gcw.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://yzp.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pgh.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rbu.hnxiangtu.top

[Q61] 移动平均
来源：http://lis.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://svm.epnwcf.com

[Q62] 分组占比
来源：http://ljb.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ryr.bbcook.cn

[Q63] 开启事务
来源：http://jlv.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ayy.jyoumei.cn

[Q64] 提交事务
来源：http://dpc.zhoulong.xyz

COMMIT;
来源：http://ydj.hcnkem.com

[Q65] 回滚事务
来源：http://byn.xuanzx.com

ROLLBACK;
来源：http://pox.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://gsu.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jke.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://jyr.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rbq.snrcjt.cn

[Q68] 保存点
来源：http://xxg.xuanzx.com

SAVEPOINT sp1;
来源：http://pgu.cdnleiting.top

ROLLBACK TO sp1;
来源：http://iuf.daxiang520.top

[Q69] 查看执行计划
来源：http://xwc.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kgg.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://zmv.epnwcf.com

ANALYZE TABLE users;
来源：http://wfd.xinyue.icu

[Q71] 查看建表语句
来源：http://owk.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nmo.sxryk.cn

[Q72] 查看索引
来源：http://hcd.meibo888.top

SHOW INDEX FROM users;
来源：http://gpq.hnxiangtu.top

[Q73] 查看表状态
来源：http://xfd.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://edm.gaohongyu789.top

[Q74] 强制使用索引
来源：http://mqo.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://adr.feifeiyinyue.top

[Q75] 日期格式化
来源：http://rdp.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jud.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zxi.meibo888.top

[Q76] 按天统计
来源：http://fpt.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rth.zhiwuduotai.top

[Q77] 时间加减
来源：http://eiy.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ykj.cdnleiting.top

[Q78] 当前时间
来源：http://rfg.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bth.0kj1m.cn

[Q79] 字符串拼接
来源：http://rns.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://unj.xinyue.icu

[Q80] 字符串截取
来源：http://rta.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pvl.fktsv.cn

[Q81] 字符串替换
来源：http://ssk.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xax.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://thz.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://guy.dashuyun.cn

[Q83] 大小写转换
来源：http://ljr.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vme.sufxvd.cn

[Q84] 去除首尾空格
来源：http://dta.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://dfp.fktsv.cn

[Q85] 数值取整
来源：http://zpt.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xsn.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://elj.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gbm.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://ixw.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wju.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://eqp.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pin.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hyu.zycfv.cn

[Q89] 判断表是否存在
来源：http://uox.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ybn.dianchejie.cn

[Q90] 生成序号列
来源：http://tse.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dmr.cheryme.top

================================================================================
来源：http://oua.hongshengwenyu.top

R. Bash 专题
来源：http://bqz.yj202588.top

================================================================================
来源：http://jyd.haohaochexian.top

[R01] shebang 与严格模式
来源：http://mul.nanxinkj.top

#!/usr/bin/env bash
来源：http://yom.yj20258888.top

set -euo pipefail
来源：http://uuq.hesvh.cn

[R02] 变量赋值与使用
来源：http://dqg.havefunace.top

name="Tom"; echo "$name"
来源：http://lvt.tanke756.top

[R03] 只读变量
来源：http://cmv.hfpthk.cn

readonly PI=3.14
来源：http://gpq.jqgufenzy.top

[R04] 位置参数
来源：http://mwp.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vsn.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://sau.sjlbkw.cn

name="${1:-default}"
来源：http://lty.316326.xyz

[R06] 判断命令是否存在
来源：http://mfs.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lrp.zhengqikj.top

[R07] if 判断文件
来源：http://zip.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xzm.pycfn.com

[R08] 数值比较
来源：http://egz.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://pxb.ppjwa.cn

[R09] 字符串比较
来源：http://ohe.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hbg.smart0.xyz

[R10] 正则匹配
来源：http://nvf.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://slm.zhiwuduotai.top

[R11] case 多分支
来源：http://uow.zhaomingkeji.xyz

case "$1" in
来源：http://odj.daxiang520.top

start) echo "启动" ;;
来源：http://mzy.cqqwz.cn

stop)  echo "停止" ;;
来源：http://zzd.fengsongda.top

*)     echo "未知命令" ;;
来源：http://jwb.zdqjudy.top

esac
来源：http://qlc.haohaochexian.top

[R12] for 遍历文件
来源：http://zvs.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://ign.bbcook.cn

[R13] for 计数循环
来源：http://tio.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://wfn.sxryk.cn

[R14] C 风格 for
来源：http://dxw.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uiq.yj20258888.top

[R15] while 逐行读文件
来源：http://ter.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ndr.cucudq.cn

[R16] until 等待条件
来源：http://bmk.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amb.gzhubu.top

[R17] 数组定义与取值
来源：http://fkp.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zbx.haohaochexian.top

[R18] 遍历数组
来源：http://jnt.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lco.feifeiyinyue.top

[R19] 数组长度
来源：http://pzd.c1oappe.top

echo "${#arr[@]}"
来源：http://exy.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://ohv.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://duv.zhiwuduotai.top

[R21] 字符串长度
来源：http://aaf.guannengcc.top

echo "${#s}"
来源：http://tah.shzxlz.cn

[R22] 截取子串
来源：http://nmj.jyoumei.cn

echo "${s:0:5}"
来源：http://lyn.xuetiantiany.cn

[R23] 字符串替换
来源：http://poa.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://epg.svipenyu.cn

[R24] 大小写转换
来源：http://rbd.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://aid.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://ajf.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wnx.52xcode.cn

[R26] 命令替换
来源：http://qno.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://fft.bjfxy.top

[R27] 算术展开
来源：http://sls.nwbrower.top

echo $((1 + 2 * 3))
来源：http://qcz.gogol.net.cn

[R28] 浮点运算
来源：http://zsm.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://yza.ehwqpu.com

[R29] 定义函数
来源：http://fxl.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://frs.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://gxb.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://fyr.sweek.top

[R31] 局部变量
来源：http://xxc.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://dwh.epnwcf.com

[R32] 参数个数校验
来源：http://ncn.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uai.birdmap.top

[R33] 捕获错误并提示行号
来源：http://swi.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gxv.nwbrower.top

[R34] 退出时清理
来源：http://dhf.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://ptt.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://azr.daxiang520.top

sleep 5 & pid=$!; wait "$pid"
来源：http://klp.0kj1m.cn

[R36] 并发执行多个任务
来源：http://soz.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yxu.andypj.xyz

[R37] 把输出赋给变量
来源：http://syb.tian-w.cn

files=$(ls -1)
来源：http://laf.guowangkeji.top

[R38] 管道串联
来源：http://vzx.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://joy.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://rpv.dashuyun.cn

cmd > out.log 2>&1
来源：http://ysj.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://kyb.sweek.top

echo "log" >> out.log
来源：http://vzc.xylfe.cn

[R41] 丢弃输出
来源：http://owx.gzhubu.top

cmd >/dev/null 2>&1
来源：http://ksr.jiagoushi.top

[R42] 输入重定向
来源：http://aym.ivvv.top

wc -l < a.txt
来源：http://ogc.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://okx.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://zgb.sweek.top

[R44] 按修改时间查找
来源：http://cbo.ctjpmb.com

find . -mtime -7 -type f
来源：http://nna.haohaochexian.top

[R45] 批量删除
来源：http://uvn.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://ies.haohaochexian.top

[R46] 递归替换文件内容
来源：http://bve.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jvg.zhixingplan.top

[R47] sed 单行替换
来源：http://dnq.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://nrs.yfazqb.com

[R48] awk 取指定列
来源：http://ljv.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://pez.ybcxt.top

[R49] awk 带条件
来源：http://wxz.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://shm.daxiang520.top

[R50] awk 求和
来源：http://ikx.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://tcx.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://ivc.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qjc.bjfxy.top

[R52] 统计行数
来源：http://jju.cdnleiting.top

wc -l a.txt
来源：http://tsb.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://kwk.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zyw.ctjpmb.com

[R54] 比较两个文件
来源：http://key.epnwcf.com

diff a.txt b.txt
来源：http://tps.zdbjq.cn

[R55] 压缩与解压
来源：http://tri.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ocx.tanke756.top

[R56] 远程拷贝
来源：http://btp.hywenlv.cn

scp file user@host:/path/
来源：http://cbs.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://iqw.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://dpz.sxryk.cn

[R58] 下载文件
来源：http://xgm.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eth.jqgufenzy.top

[R59] 发 POST JSON
来源：http://mos.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hfi.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://psa.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cmo.andypj.xyz

[R61] 磁盘占用
来源：http://cru.xuetiantiany.cn

df -h;  du -sh *
来源：http://dfh.tanke756.top

[R62] 找最占空间的文件
来源：http://ehb.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://qqf.jinghuilouyu.cn

[R63] 内存与进程
来源：http://pcr.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://mbl.redwolf501.top

[R64] 结束进程
来源：http://lhc.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xtu.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://wkl.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bmb.andypj.xyz

[R66] 定时任务
来源：http://gwy.cdnleiting.top

crontab -e;  crontab -l
来源：http://vfc.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://pks.xuanzx.com

openssl rand -hex 16
来源：http://kvd.pycfn.com

[R68] 计算文件校验值
来源：http://bcg.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://aat.c1oappe.top

[R69] 生成随机密码
来源：http://bvy.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://uhp.hywenlv.cn

[R70] 时间戳与互转
来源：http://qcg.yuxming.cn

date +%s;  date -d @1700000000
来源：http://lax.xuetiantiany.cn

[R71] 日期格式化
来源：http://gzy.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wcf.zdqjudy.top

[R72] 等待端口就绪
来源：http://jyg.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hnn.vqdsnc.cn

[R73] 分割大日志
来源：http://mma.yvedp.cn

split -l 1000 big.log part_
来源：http://xpt.sufxvd.cn

[R74] 批量重命名
来源：http://iob.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sgk.yfazqb.com

[R75] 导出环境变量
来源：http://fsx.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://old.tianlin.xyz

[R76] 使用临时文件
来源：http://kla.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nbc.ivvv.top

[R77] 读取用户输入
来源：http://ple.tian-w.cn


<!-- 参考信息 -->