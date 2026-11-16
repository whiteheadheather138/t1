代发 wailian999

[Q33] 多列分组
来源：http://dmr.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nhm.zdbjq.cn

[Q34] 每组取第一条
来源：http://mgx.chenlongwang.top

SELECT * FROM (
来源：http://trf.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://slh.bjfxy.top

) t WHERE rn = 1;
来源：http://phm.ybcxt.top

[Q35] 内连接
来源：http://bux.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://leo.jinghuilouyu.cn

[Q36] 左连接
来源：http://mgz.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lzq.birdmap.top

[Q37] 右连接
来源：http://ihb.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ckh.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://spn.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pqu.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://sqv.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xho.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zke.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vid.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xbc.fengsongda.top

[Q41] 多表连接
来源：http://iyh.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qpf.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://xgj.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://iol.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://hjc.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://rkt.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpr.yonumen.top

[Q43] 标量子查询
来源：http://dwx.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xcx.havefunace.top

[Q44] IN 子查询
来源：http://pyk.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lma.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://onz.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ypz.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jea.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqt.zhengqikj.top

[Q47] 与平均值比较
来源：http://vuw.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pka.316326.xyz

[Q48] CTE 公用表表达式
来源：http://cmg.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zxj.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://pwj.aizwys.cn

[Q49] 更新单行
来源：http://lni.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hiu.chenzaomai.com

[Q50] 批量更新
来源：http://ekl.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hfu.316326.xyz

[Q51] 用子查询更新
来源：http://nmu.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wkx.xinyue.icu

[Q52] 删除指定行
来源：http://rhf.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://kgl.fengsongda.top

[Q53] 按条件删除
来源：http://pca.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lnp.tanke756.top

[Q54] 清空表
来源：http://qyu.vehdjk.com

TRUNCATE TABLE logs;
来源：http://snl.xinyue.icu

[Q55] 排名（并列占位）
来源：http://nqt.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://een.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://rdv.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gzl.guowangkeji.top

[Q57] 行号
来源：http://wbr.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fml.cheryme.top

[Q58] 累计求和
来源：http://qmg.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwv.shuidangran.top

[Q59] 分组内累计
来源：http://ocw.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sao.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://kxa.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lry.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sxd.quarkkingdee.top

[Q61] 移动平均
来源：http://sgv.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://spd.cucudq.cn

[Q62] 分组占比
来源：http://sei.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iuw.sysykeji.top

[Q63] 开启事务
来源：http://yui.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hmd.nwbrower.top

[Q64] 提交事务
来源：http://lmc.haohaochexian.top

COMMIT;
来源：http://rxt.nanxuanxn.top

[Q65] 回滚事务
来源：http://feb.guowangkeji.top

ROLLBACK;
来源：http://lvx.ydzc1.top

[Q66] 行锁查询
来源：http://hbc.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dud.guowangkeji.top

[Q67] 设置隔离级别
来源：http://dzn.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvn.jinyuanbaomall.cn

[Q68] 保存点
来源：http://jxb.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://rpv.shuidangran.top

ROLLBACK TO sp1;
来源：http://qfp.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://dfj.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xmb.guowangkeji.top

[Q70] 更新统计信息
来源：http://grz.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://ibs.sysykeji.top

[Q71] 查看建表语句
来源：http://epq.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yyz.jyoumei.cn

[Q72] 查看索引
来源：http://njz.316326.xyz

SHOW INDEX FROM users;
来源：http://jyl.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://wrz.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mqv.cdnleiting.top

[Q74] 强制使用索引
来源：http://jrs.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wwz.cucudq.cn

[Q75] 日期格式化
来源：http://wki.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://leu.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tot.0kj1m.cn

[Q76] 按天统计
来源：http://rpt.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pva.pengpengdd.cyou

[Q77] 时间加减
来源：http://nav.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tsg.yuxming.cn

[Q78] 当前时间
来源：http://ged.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qwp.pycfn.com

[Q79] 字符串拼接
来源：http://osw.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lnc.sufxvd.cn

[Q80] 字符串截取
来源：http://wqu.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://twt.yj20258888.top

[Q81] 字符串替换
来源：http://heh.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rfl.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://ovz.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hru.xziqi.cn

[Q83] 大小写转换
来源：http://edl.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oae.uphjek.com

[Q84] 去除首尾空格
来源：http://wgc.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://plv.hcnkem.com

[Q85] 数值取整
来源：http://ayw.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zul.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://oev.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://npd.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://zej.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dqd.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://kex.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mzm.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uxs.ehwqpu.com

[Q89] 判断表是否存在
来源：http://yuz.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://izu.uphjek.com

[Q90] 生成序号列
来源：http://vnz.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyk.smart0.xyz

================================================================================
来源：http://vuj.jlsjyb.cn

R. Bash 专题
来源：http://cxg.xingfuxueyuan.xyz

================================================================================
来源：http://mtp.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://giu.fengsongda.top

#!/usr/bin/env bash
来源：http://oiu.xuetiantiany.cn

set -euo pipefail
来源：http://udb.shuidangran.top

[R02] 变量赋值与使用
来源：http://kng.fehbvm.com

name="Tom"; echo "$name"
来源：http://wod.smart0.xyz

[R03] 只读变量
来源：http://edd.andypj.xyz

readonly PI=3.14
来源：http://doh.aibaodan.cn

[R04] 位置参数
来源：http://ljg.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gmo.meibo888.top

[R05] 参数默认值
来源：http://qly.yfazqb.com

name="${1:-default}"
来源：http://emf.cheryme.top

[R06] 判断命令是否存在
来源：http://afj.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ebb.daria6918.cn

[R07] if 判断文件
来源：http://dei.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lxu.epnwcf.com

[R08] 数值比较
来源：http://thd.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jlp.shanyushiyangtech.top

[R09] 字符串比较
来源：http://opa.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rsl.chenzaomai.com

[R10] 正则匹配
来源：http://lhb.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gis.hywenlv.cn

[R11] case 多分支
来源：http://bws.wangdashe.top

case "$1" in
来源：http://tdm.52xcode.cn

start) echo "启动" ;;
来源：http://tzy.yangfankeji.com

stop)  echo "停止" ;;
来源：http://iay.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://zjg.yongpay.top

esac
来源：http://fsz.cheryme.top

[R12] for 遍历文件
来源：http://zqy.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://sjo.yuanzhike.top

[R13] for 计数循环
来源：http://xbv.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://bqw.xuanzx.com

[R14] C 风格 for
来源：http://elz.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oob.yueranfly.top

[R15] while 逐行读文件
来源：http://riq.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bgn.ehwqpu.com

[R16] until 等待条件
来源：http://dst.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pbc.fengsongda.top

[R17] 数组定义与取值
来源：http://xmw.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pyk.chenzaomai.com

[R18] 遍历数组
来源：http://tez.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nwm.yj20258888.top

[R19] 数组长度
来源：http://yza.birdmap.top

echo "${#arr[@]}"
来源：http://vrb.hnqzz.top

[R20] 关联数组（字典）
来源：http://lrn.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pys.gogol.net.cn

[R21] 字符串长度
来源：http://rwp.jinqigfzy.top

echo "${#s}"
来源：http://oyr.daxiang520.top

[R22] 截取子串
来源：http://kyn.ybcxt.top

echo "${s:0:5}"
来源：http://zkl.jqgfzy.top

[R23] 字符串替换
来源：http://tbo.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qhv.nanxuanxn.top

[R24] 大小写转换
来源：http://rpf.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qoc.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://zqz.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://lce.ywan-chungtsiang.top

[R26] 命令替换
来源：http://ehb.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://qnf.zdqjudy.top

[R27] 算术展开
来源：http://avn.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://bjj.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://axs.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://ubs.zhaomingkeji.xyz

[R29] 定义函数
来源：http://npj.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sjt.zdqjudy.top

[R30] 函数返回状态码
来源：http://tjm.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lhc.andypj.xyz

[R31] 局部变量
来源：http://rzd.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://ltv.yueranfly.top

[R32] 参数个数校验
来源：http://oee.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qle.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://ecf.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gma.hysaishi.cn

[R34] 退出时清理
来源：http://ryb.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nsm.c1oappe.top

[R35] 后台执行并等待
来源：http://dad.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ebc.jiagoushi.top

[R36] 并发执行多个任务
来源：http://hjl.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://utx.jiagoushi.top

[R37] 把输出赋给变量
来源：http://yje.mhx1999.top

files=$(ls -1)
来源：http://ezj.smart0.xyz

[R38] 管道串联
来源：http://btn.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://bfz.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://fbk.sweek.top

cmd > out.log 2>&1
来源：http://mcq.zhiwuduotai.top

[R40] 追加写日志
来源：http://tby.andypj.xyz

echo "log" >> out.log
来源：http://tlr.pengpengdd.cyou

[R41] 丢弃输出
来源：http://coi.fengsongda.top

cmd >/dev/null 2>&1
来源：http://xwz.birdmap.top

[R42] 输入重定向
来源：http://bsv.wangshuangyany.cn

wc -l < a.txt
来源：http://wuw.cdnleiting.top

[R43] 按名字查找文件
来源：http://gav.redwolf501.top

find . -name "*.log" -type f
来源：http://jgb.ybcxt.top

[R44] 按修改时间查找
来源：http://xqt.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://thu.zdqjudy.top

[R45] 批量删除
来源：http://ton.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://qhd.birdmap.top

[R46] 递归替换文件内容
来源：http://krf.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fcf.ctjpmb.com

[R47] sed 单行替换
来源：http://cga.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://aep.chenlongwang.top

[R48] awk 取指定列
来源：http://wmc.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://xsp.tianlin.xyz

[R49] awk 带条件
来源：http://dcs.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dye.tianlin.xyz

[R50] awk 求和
来源：http://eis.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wno.dashuyun.cn

[R51] 排序去重取前几
来源：http://skz.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://klb.yueranfly.top

[R52] 统计行数
来源：http://mol.hywenlv.cn

wc -l a.txt
来源：http://tzz.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://sbh.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fqh.yj202588.top

[R54] 比较两个文件
来源：http://stn.daxiang520.top

diff a.txt b.txt
来源：http://ojg.chenlongwang.top

[R55] 压缩与解压
来源：http://xgj.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wti.hysaishi.cn

[R56] 远程拷贝
来源：http://xmp.jlsjyb.cn

scp file user@host:/path/
来源：http://qnu.jinqigufen.top

[R57] 远程执行命令
来源：http://rul.tanke756.top

ssh user@host 'uptime'
来源：http://biy.jinqigufen.top

[R58] 下载文件
来源：http://bge.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uzi.vqdsnc.cn

[R59] 发 POST JSON
来源：http://wfs.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bkz.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://mdv.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ixz.ivvv.top

[R61] 磁盘占用
来源：http://jpa.redwolf501.top

df -h;  du -sh *
来源：http://mgm.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://wqm.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://nbi.hcnkem.com

[R63] 内存与进程
来源：http://pgu.316326.xyz

free -h;  ps aux | grep nginx
来源：http://rdn.jqgufenzy.top

[R64] 结束进程
来源：http://jkt.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://wph.shzxlz.cn

[R65] 查看端口占用
来源：http://fft.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://auq.smart0.xyz

[R66] 定时任务
来源：http://ras.9152youxi.cn

crontab -e;  crontab -l
来源：http://gjv.mhx1999.top

[R67] 生成随机十六进制串
来源：http://cjd.ppjwa.cn

openssl rand -hex 16
来源：http://fqu.ybcxt.top

[R68] 计算文件校验值
来源：http://yfh.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aop.xuetiantiany.cn

[R69] 生成随机密码
来源：http://har.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://hin.yangfankeji.com

[R70] 时间戳与互转
来源：http://fpt.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://ffq.quarkkingdee.top

[R71] 日期格式化
来源：http://lvp.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ctd.guannengcc.top

[R72] 等待端口就绪
来源：http://uwo.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://bgz.ppjwa.cn

[R73] 分割大日志
来源：http://ioo.bbcook.cn

split -l 1000 big.log part_
来源：http://dvs.yj20258888.top

[R74] 批量重命名
来源：http://ezu.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://api.yangfankeji.com

[R75] 导出环境变量
来源：http://tdp.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://knb.gzhubu.top

[R76] 使用临时文件
来源：http://xmq.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kah.feifeiyinyue.top

[R77] 读取用户输入
来源：http://obc.vehdjk.com

read -rp "请输入: " ans
来源：http://dvo.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://ama.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wqj.cdnleiting.top

[R79] 解析命令行选项
来源：http://ouj.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gks.uphjek.com

[R80] 查看脚本执行耗时
来源：http://vmk.ppjwa.cn

time ./run.sh
来源：http://rdy.kuanghao11.cn

================================================================================
来源：http://ouq.xylfe.cn

S. C / C++ 专题
来源：http://dhy.ivvv.top

================================================================================
来源：http://wbm.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://jdn.ehwqpu.com

#include <stdio.h>
来源：http://rpt.tianlin.xyz


<!-- 参考信息 -->