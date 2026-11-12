代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://btp.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://glt.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://ezb.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rec.fktsv.cn

[Q36] 左连接
来源：http://pqz.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dfe.zdbjq.cn

[Q37] 右连接
来源：http://aim.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mpc.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://wni.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mie.cashguo.top

[Q39] 自连接（查上下级）
来源：http://tvw.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nyr.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ncs.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tqw.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqx.jqgfzy.top

[Q41] 多表连接
来源：http://xhk.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sff.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://axb.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://hbe.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://cib.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://zkd.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vtn.jqgufenzy.top

[Q43] 标量子查询
来源：http://xrj.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vaw.yvedp.cn

[Q44] IN 子查询
来源：http://ulf.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vfg.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://poz.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ghk.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dxv.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvu.xuanzx.com

[Q47] 与平均值比较
来源：http://ahg.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dxq.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://xzz.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dzk.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://sws.jyoumei.cn

[Q49] 更新单行
来源：http://wvs.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gdm.jinqigufen.top

[Q50] 批量更新
来源：http://tlt.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zvt.cdnleiting.top

[Q51] 用子查询更新
来源：http://snf.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rzg.jqgfzy.top

[Q52] 删除指定行
来源：http://yam.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://gwg.uphjek.com

[Q53] 按条件删除
来源：http://ybb.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nmp.ydzc1.top

[Q54] 清空表
来源：http://zmn.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://mka.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://jkt.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ibs.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://qrr.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fxr.jinyuanbaomall.cn

[Q57] 行号
来源：http://wcd.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://owa.gzhubu.top

[Q58] 累计求和
来源：http://xxk.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oiv.epnwcf.com

[Q59] 分组内累计
来源：http://jkf.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wek.sweek.top

[Q60] 取上一行 / 下一行
来源：http://zbc.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qrv.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dnr.xuanzx.com

[Q61] 移动平均
来源：http://jcz.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bla.dashuyun.cn

[Q62] 分组占比
来源：http://yos.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lsd.kuanghao11.cn

[Q63] 开启事务
来源：http://liv.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nky.fanxiaobao.xyz

[Q64] 提交事务
来源：http://rck.ivvv.top

COMMIT;
来源：http://ipg.ppjwa.cn

[Q65] 回滚事务
来源：http://gel.xingfuxueyuan.xyz

ROLLBACK;
来源：http://stv.sysykeji.top

[Q66] 行锁查询
来源：http://sse.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://niv.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://kgf.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qtp.chenlongwang.top

[Q68] 保存点
来源：http://rhm.yuxming.cn

SAVEPOINT sp1;
来源：http://gjv.zdbjq.cn

ROLLBACK TO sp1;
来源：http://nps.316326.xyz

[Q69] 查看执行计划
来源：http://oxv.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://knz.316326.xyz

[Q70] 更新统计信息
来源：http://nmt.ivvv.top

ANALYZE TABLE users;
来源：http://slg.nwbrower.top

[Q71] 查看建表语句
来源：http://tcq.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eno.uphjek.com

[Q72] 查看索引
来源：http://sjg.mhx1999.top

SHOW INDEX FROM users;
来源：http://wbi.vqdsnc.cn

[Q73] 查看表状态
来源：http://vur.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jto.iojbl.cn

[Q74] 强制使用索引
来源：http://jqh.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sji.chenzaomai.com

[Q75] 日期格式化
来源：http://eaz.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ywi.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mie.hywenlv.cn

[Q76] 按天统计
来源：http://uem.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yjx.jinghuilouyu.cn

[Q77] 时间加减
来源：http://dew.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hzg.yj202588.top

[Q78] 当前时间
来源：http://eeo.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ouq.gotoacloud.top

[Q79] 字符串拼接
来源：http://aek.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hcs.jiagoushi.top

[Q80] 字符串截取
来源：http://ujv.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ooq.nanxinkj.top

[Q81] 字符串替换
来源：http://lrp.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bha.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://zyr.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://usm.hesvh.cn

[Q83] 大小写转换
来源：http://ebg.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bat.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://zko.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://cwc.cashguo.top

[Q85] 数值取整
来源：http://wxa.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zes.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://sdl.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iiv.yongpay.top

[Q87] JSON 字段做条件
来源：http://lnk.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rem.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://wek.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ghy.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jvm.haohaochexian.top

[Q89] 判断表是否存在
来源：http://wtm.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vgs.ivvv.top

[Q90] 生成序号列
来源：http://pie.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://phi.hesvh.cn

================================================================================
来源：http://jol.aizwys.cn

R. Bash 专题
来源：http://bxd.zhixingplan.top

================================================================================
来源：http://cee.bjfxy.top

[R01] shebang 与严格模式
来源：http://bum.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://ikh.yj202588.top

set -euo pipefail
来源：http://vvy.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://pyn.yj20258888.top

name="Tom"; echo "$name"
来源：http://kby.cashguo.top

[R03] 只读变量
来源：http://iud.yongpay.top

readonly PI=3.14
来源：http://dwo.hammf.cn

[R04] 位置参数
来源：http://uht.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yum.yangfankeji.com

[R05] 参数默认值
来源：http://iif.svipenyu.cn

name="${1:-default}"
来源：http://jhw.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://vwh.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mvm.9152youxi.cn

[R07] if 判断文件
来源：http://ugs.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uli.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://zar.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ovc.yongpay.top

[R09] 字符串比较
来源：http://azx.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pff.sxryk.cn

[R10] 正则匹配
来源：http://cwm.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fvc.jyoumei.cn

[R11] case 多分支
来源：http://noi.gogol.net.cn

case "$1" in
来源：http://sgh.nanxinkj.top

start) echo "启动" ;;
来源：http://fln.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://uar.wangdashe.top

*)     echo "未知命令" ;;
来源：http://uxr.daxiang520.top

esac
来源：http://rwm.xuetiantiany.cn

[R12] for 遍历文件
来源：http://iss.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://iit.cqqwz.cn

[R13] for 计数循环
来源：http://dkr.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://yyo.yj20258888.top

[R14] C 风格 for
来源：http://thh.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pmq.sxryk.cn

[R15] while 逐行读文件
来源：http://eja.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zrl.jiagoushi.top

[R16] until 等待条件
来源：http://fry.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tnf.sjlbkw.cn

[R17] 数组定义与取值
来源：http://akw.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://miq.birdmap.top

[R18] 遍历数组
来源：http://hbt.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bwu.pengpengdd.cyou

[R19] 数组长度
来源：http://ukb.zhijiandao.cn

echo "${#arr[@]}"
来源：http://hod.yongpay.top

[R20] 关联数组（字典）
来源：http://dfa.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ddd.ivvv.top

[R21] 字符串长度
来源：http://qyh.zhiwuduotai.top

echo "${#s}"
来源：http://epe.chenlongwang.top

[R22] 截取子串
来源：http://xcb.cqqwz.cn

echo "${s:0:5}"
来源：http://evl.uphjek.com

[R23] 字符串替换
来源：http://mkz.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yad.zdbjq.cn

[R24] 大小写转换
来源：http://ndi.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ezq.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ljq.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kob.cashguo.top

[R26] 命令替换
来源：http://wml.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://mlq.zhixingplan.top

[R27] 算术展开
来源：http://fmm.bjfxy.top

echo $((1 + 2 * 3))
来源：http://wkj.ctjpmb.com

[R28] 浮点运算
来源：http://wqw.sweek.top

echo "scale=2; 10/3" | bc
来源：http://iht.xuetiantiany.cn

[R29] 定义函数
来源：http://vot.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gyy.sjlbkw.cn

[R30] 函数返回状态码
来源：http://oax.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://pmd.havefunace.top

[R31] 局部变量
来源：http://hdd.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://lmh.gzhubu.top

[R32] 参数个数校验
来源：http://ihx.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kjx.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://lua.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nem.hnqzz.top

[R34] 退出时清理
来源：http://rhl.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://kvf.yuanzhike.top

[R35] 后台执行并等待
来源：http://ndf.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jpe.cashguo.top

[R36] 并发执行多个任务
来源：http://azl.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://npr.yonumen.top

[R37] 把输出赋给变量
来源：http://xbw.snrcjt.cn

files=$(ls -1)
来源：http://vrn.jlsjyb.cn

[R38] 管道串联
来源：http://kev.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://vzb.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://sfy.daria6918.cn

cmd > out.log 2>&1
来源：http://tjm.zdqjudy.top

[R40] 追加写日志
来源：http://zjv.hfpthk.cn

echo "log" >> out.log
来源：http://vdk.bbcook.cn

[R41] 丢弃输出
来源：http://rpw.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://yuu.svipenyu.cn

[R42] 输入重定向
来源：http://sil.jlsjyb.cn

wc -l < a.txt
来源：http://sye.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://cyt.zdqjudy.top

find . -name "*.log" -type f
来源：http://hdn.chenlongwang.top

[R44] 按修改时间查找
来源：http://fky.yfazqb.com

find . -mtime -7 -type f
来源：http://xuq.gzhubu.top

[R45] 批量删除
来源：http://jzh.jianghu66.top

find . -name "*.tmp" -delete
来源：http://lju.yvedp.cn

[R46] 递归替换文件内容
来源：http://gre.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qsg.jyoumei.cn

[R47] sed 单行替换
来源：http://hei.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://rcn.hnqzz.top

[R48] awk 取指定列
来源：http://kgv.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://faq.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://szy.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tdv.dashuyun.cn

[R50] awk 求和
来源：http://qsx.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://cwq.ybcxt.top

[R51] 排序去重取前几
来源：http://uvc.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://elj.hongshengwenyu.top

[R52] 统计行数
来源：http://cul.cqqwz.cn

wc -l a.txt
来源：http://jra.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://rql.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cub.wangshuangyany.cn

[R54] 比较两个文件
来源：http://fyx.0kj1m.cn

diff a.txt b.txt
来源：http://ubj.dashuyun.cn

[R55] 压缩与解压
来源：http://okq.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eqt.sufxvd.cn

[R56] 远程拷贝
来源：http://zeq.cheryme.top

scp file user@host:/path/
来源：http://uck.jiagoushi.top

[R57] 远程执行命令
来源：http://wpd.hcnkem.com

ssh user@host 'uptime'
来源：http://uyw.smart0.xyz

[R58] 下载文件
来源：http://kqo.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://shb.ybcxt.top

[R59] 发 POST JSON
来源：http://klr.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://urf.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://mss.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zzz.hcnkem.com

[R61] 磁盘占用
来源：http://edy.wangshuangyany.cn

df -h;  du -sh *
来源：http://tqb.mhx1999.top

[R62] 找最占空间的文件
来源：http://epq.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://ebo.316326.xyz

[R63] 内存与进程
来源：http://dtk.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://ste.chenjidiqi.icu

[R64] 结束进程
来源：http://csg.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://dzx.tian-w.cn

[R65] 查看端口占用
来源：http://edv.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dza.yfazqb.com

[R66] 定时任务
来源：http://fxm.tian-w.cn

crontab -e;  crontab -l
来源：http://oha.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://aru.daria6918.cn

openssl rand -hex 16
来源：http://dyc.hammf.cn

[R68] 计算文件校验值
来源：http://mhk.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ouh.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://djj.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://zba.snrcjt.cn

[R70] 时间戳与互转
来源：http://rrv.fktsv.cn

date +%s;  date -d @1700000000
来源：http://pfr.zdqjudy.top

[R71] 日期格式化
来源：http://vee.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mmt.jqgfzy.top

[R72] 等待端口就绪
来源：http://ofn.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ohi.ydzc1.top

[R73] 分割大日志
来源：http://xsx.ybcxt.top

split -l 1000 big.log part_
来源：http://qwp.shanyushiyangtech.top

[R74] 批量重命名
来源：http://oot.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vjh.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://hup.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://uhp.nwbrower.top

[R76] 使用临时文件
来源：http://ghj.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gum.zhoulong.xyz

[R77] 读取用户输入
来源：http://uye.hammf.cn

read -rp "请输入: " ans
来源：http://kyj.xziqi.cn

[R78] 交互式菜单
来源：http://kie.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://may.xylfe.cn

[R79] 解析命令行选项
来源：http://gwv.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kjo.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://vhp.zycfv.cn

time ./run.sh
来源：http://cro.zhiwuduotai.top

================================================================================
来源：http://doj.tanke756.top

S. C / C++ 专题
来源：http://xmd.yongpay.top

================================================================================
来源：http://lsz.shzxlz.cn

[S01] C：Hello World
来源：http://yrk.sxryk.cn

#include <stdio.h>
来源：http://bfr.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oxf.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://btq.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://jau.pengpengdd.cyou

[S03] C：读入整数
来源：http://nqv.nanxinkj.top


<!-- 参考信息 -->