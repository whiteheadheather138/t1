代发 wailian999

[Q33] 多列分组
来源：http://vyc.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vlv.havefunace.top

[Q34] 每组取第一条
来源：http://qru.hnqzz.top

SELECT * FROM (
来源：http://xiy.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rrx.jqgfzy.top

) t WHERE rn = 1;
来源：http://hvj.tarul.cn

[Q35] 内连接
来源：http://hky.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gsp.jyoumei.cn

[Q36] 左连接
来源：http://csn.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ccj.shanyushiyangkeji.top

[Q37] 右连接
来源：http://kqa.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zwf.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xok.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dme.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://sia.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gis.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iyg.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zvd.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qjs.ybcxt.top

[Q41] 多表连接
来源：http://wsa.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zbi.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://jhf.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://fnr.tarul.cn

[Q42] 连接条件附加过滤
来源：http://tdl.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://oox.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tjm.xuetiantiany.cn

[Q43] 标量子查询
来源：http://mgs.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kkk.gotoacloud.top

[Q44] IN 子查询
来源：http://udi.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://poi.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://xtw.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jqe.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://lah.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hfn.sxryk.cn

[Q47] 与平均值比较
来源：http://qxx.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://egt.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://jmq.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ixe.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://wvh.zhoulong.xyz

[Q49] 更新单行
来源：http://jpi.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rpm.jinqigufen.top

[Q50] 批量更新
来源：http://mon.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jhr.52xcode.cn

[Q51] 用子查询更新
来源：http://cnt.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yqw.xylfe.cn

[Q52] 删除指定行
来源：http://rkz.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://ebv.dianchejie.cn

[Q53] 按条件删除
来源：http://imi.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nnn.svipenyu.cn

[Q54] 清空表
来源：http://gqh.316326.xyz

TRUNCATE TABLE logs;
来源：http://vxb.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://qht.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lju.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://jxp.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lyb.yj202588.top

[Q57] 行号
来源：http://lic.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ckx.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://geo.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wvy.xuanzx.com

[Q59] 分组内累计
来源：http://lrh.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lah.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://xmo.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vys.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jvm.yuxming.cn

[Q61] 移动平均
来源：http://hka.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dfw.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://dds.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nyh.yanxiufei.cn

[Q63] 开启事务
来源：http://igc.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tss.316326.xyz

[Q64] 提交事务
来源：http://dqf.gaohongyu789.top

COMMIT;
来源：http://vnt.epnwcf.com

[Q65] 回滚事务
来源：http://dkc.zhaomingkeji.xyz

ROLLBACK;
来源：http://tzs.gaohongyu789.top

[Q66] 行锁查询
来源：http://oxh.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lgn.ybcxt.top

[Q67] 设置隔离级别
来源：http://egq.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hfq.shanyushiyangkeji.top

[Q68] 保存点
来源：http://aiv.tianlin.xyz

SAVEPOINT sp1;
来源：http://pqy.epnwcf.com

ROLLBACK TO sp1;
来源：http://hup.yonumen.top

[Q69] 查看执行计划
来源：http://rcj.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wsc.svipenyu.cn

[Q70] 更新统计信息
来源：http://atv.yuanzhike.top

ANALYZE TABLE users;
来源：http://nex.gaohongyu789.top

[Q71] 查看建表语句
来源：http://tcn.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://thw.zycfv.cn

[Q72] 查看索引
来源：http://pke.52xcode.cn

SHOW INDEX FROM users;
来源：http://wmw.pengpengdd.cyou

[Q73] 查看表状态
来源：http://nsh.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mqj.dashuyun.cn

[Q74] 强制使用索引
来源：http://usc.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uar.fzhhl.top

[Q75] 日期格式化
来源：http://ekr.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://suk.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ezd.snrcjt.cn

[Q76] 按天统计
来源：http://dvw.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://whp.wangdashe.top

[Q77] 时间加减
来源：http://eom.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sqt.yangfankeji.com

[Q78] 当前时间
来源：http://ytf.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wwd.hcnkem.com

[Q79] 字符串拼接
来源：http://myz.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://orb.gogol.net.cn

[Q80] 字符串截取
来源：http://ors.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tor.vqdsnc.cn

[Q81] 字符串替换
来源：http://gtc.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kxg.yj202588.top

[Q82] 字符长度与字节长度
来源：http://mei.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://der.cashguo.top

[Q83] 大小写转换
来源：http://gms.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbw.hywenlv.cn

[Q84] 去除首尾空格
来源：http://nka.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://hxj.hywenlv.cn

[Q85] 数值取整
来源：http://aep.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dwd.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://ibe.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ged.hesvh.cn

[Q87] JSON 字段做条件
来源：http://ghu.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yyx.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://dcs.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://skj.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xhf.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://igt.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwq.cashguo.top

[Q90] 生成序号列
来源：http://qqw.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glg.cashguo.top

================================================================================
来源：http://ngc.zhengqikj.top

R. Bash 专题
来源：http://cno.pycfn.com

================================================================================
来源：http://lbh.meibo888.top

[R01] shebang 与严格模式
来源：http://nzc.bbcook.cn

#!/usr/bin/env bash
来源：http://tag.hnxiangtu.top

set -euo pipefail
来源：http://ibu.yueranfly.top

[R02] 变量赋值与使用
来源：http://nni.ppjwa.cn

name="Tom"; echo "$name"
来源：http://uzs.birdmap.top

[R03] 只读变量
来源：http://omx.jiagoushi.top

readonly PI=3.14
来源：http://rgm.yueranfly.top

[R04] 位置参数
来源：http://xob.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qll.fanxiaobao.xyz

[R05] 参数默认值
来源：http://zkc.xylfe.cn

name="${1:-default}"
来源：http://quw.chenlongwang.top

[R06] 判断命令是否存在
来源：http://lyq.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yud.yanxiufei.cn

[R07] if 判断文件
来源：http://bsl.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wbx.hfpthk.cn

[R08] 数值比较
来源：http://dor.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zwu.vqdsnc.cn

[R09] 字符串比较
来源：http://xnl.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qnq.jiagoushi.top

[R10] 正则匹配
来源：http://uwt.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pkr.daxiang520.top

[R11] case 多分支
来源：http://pst.aizwys.cn

case "$1" in
来源：http://mtd.hnqzz.top

start) echo "启动" ;;
来源：http://mdh.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://ykx.bbcook.cn

*)     echo "未知命令" ;;
来源：http://dxt.yj20258.top

esac
来源：http://dyc.yonumen.top

[R12] for 遍历文件
来源：http://ibd.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://mzw.vehdjk.com

[R13] for 计数循环
来源：http://tcv.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://ffw.redwolf501.top

[R14] C 风格 for
来源：http://raj.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vdm.ydjk.org.cn

[R15] while 逐行读文件
来源：http://ugm.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wwg.kuanghao11.cn

[R16] until 等待条件
来源：http://xtm.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mkq.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://ufx.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://lfn.tarul.cn

[R18] 遍历数组
来源：http://lui.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ecp.yueranfly.top

[R19] 数组长度
来源：http://fsq.yj20258.top

echo "${#arr[@]}"
来源：http://blc.nwbrower.top

[R20] 关联数组（字典）
来源：http://ipz.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oqi.hcnkem.com

[R21] 字符串长度
来源：http://ckr.vehdjk.com

echo "${#s}"
来源：http://hxw.sufxvd.cn

[R22] 截取子串
来源：http://ios.xuetiantiany.cn

echo "${s:0:5}"
来源：http://cto.jianghu66.top

[R23] 字符串替换
来源：http://eiz.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://amj.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://gkg.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yma.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://hak.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://fvg.yj20258.top

[R26] 命令替换
来源：http://qqi.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://jbb.daria6918.cn

[R27] 算术展开
来源：http://laz.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://iqn.yuxming.cn

[R28] 浮点运算
来源：http://phy.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://hnm.yuxming.cn

[R29] 定义函数
来源：http://ioz.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pap.gzhubu.top

[R30] 函数返回状态码
来源：http://hjz.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://sdt.hnqzz.top

[R31] 局部变量
来源：http://pmp.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://vka.ybcxt.top

[R32] 参数个数校验
来源：http://fjx.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nck.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://vcc.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gmg.sjlbkw.cn

[R34] 退出时清理
来源：http://tzu.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://rji.chenlongwang.top

[R35] 后台执行并等待
来源：http://gik.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zsj.pycfn.com

[R36] 并发执行多个任务
来源：http://oph.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gba.yueranfly.top

[R37] 把输出赋给变量
来源：http://dnx.yuxming.cn

files=$(ls -1)
来源：http://mmr.gogol.net.cn

[R38] 管道串联
来源：http://ake.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://pic.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://qyt.daria6918.cn

cmd > out.log 2>&1
来源：http://jez.pycfn.com

[R40] 追加写日志
来源：http://yzr.ehwqpu.com

echo "log" >> out.log
来源：http://byc.birdmap.top

[R41] 丢弃输出
来源：http://vgb.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://umb.sysykeji.top

[R42] 输入重定向
来源：http://xve.iojbl.cn

wc -l < a.txt
来源：http://yhb.ivvv.top

[R43] 按名字查找文件
来源：http://rnr.chenzaomai.com

find . -name "*.log" -type f
来源：http://kgo.shzxlz.cn

[R44] 按修改时间查找
来源：http://bcu.52xcode.cn

find . -mtime -7 -type f
来源：http://rcg.wangshuangyany.cn

[R45] 批量删除
来源：http://ver.c1oappe.top

find . -name "*.tmp" -delete
来源：http://imn.zhengqikj.top

[R46] 递归替换文件内容
来源：http://jct.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://joh.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://qnm.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://ijb.chenlongwang.top

[R48] awk 取指定列
来源：http://rym.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://kje.nwbrower.top

[R49] awk 带条件
来源：http://nxa.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dbf.316326.xyz

[R50] awk 求和
来源：http://shl.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://red.epnwcf.com

[R51] 排序去重取前几
来源：http://vgz.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://wmj.fktsv.cn

[R52] 统计行数
来源：http://zut.cheryme.top

wc -l a.txt
来源：http://xuo.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://fpv.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ags.zhoulong.xyz

[R54] 比较两个文件
来源：http://bca.52xcode.cn

diff a.txt b.txt
来源：http://qkv.52xcode.cn

[R55] 压缩与解压
来源：http://zkf.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://imi.bbcook.cn

[R56] 远程拷贝
来源：http://dvh.zdbjq.cn

scp file user@host:/path/
来源：http://qtx.daxiang520.top

[R57] 远程执行命令
来源：http://ydq.jqgufenzy.top

ssh user@host 'uptime'
来源：http://txw.bjfxy.top

[R58] 下载文件
来源：http://rjd.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pft.chenzaomai.com

[R59] 发 POST JSON
来源：http://xha.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://keo.sweek.top

[R60] 只看 HTTP 状态码
来源：http://egu.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qlr.zdbjq.cn

[R61] 磁盘占用
来源：http://ukv.ivvv.top

df -h;  du -sh *
来源：http://oyd.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://cxv.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://ojh.yj20258.top

[R63] 内存与进程
来源：http://sza.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://lkn.sxryk.cn

[R64] 结束进程
来源：http://rnf.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://jlj.yanxiufei.cn

[R65] 查看端口占用
来源：http://iyd.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wcs.jinqigufen.top

[R66] 定时任务
来源：http://avi.gzhubu.top

crontab -e;  crontab -l
来源：http://wbi.aizwys.cn

[R67] 生成随机十六进制串
来源：http://aqm.zhixingplan.top

openssl rand -hex 16
来源：http://uyn.fktsv.cn

[R68] 计算文件校验值
来源：http://rkm.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://sho.zhijiandao.cn

[R69] 生成随机密码
来源：http://ava.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://jye.chenzaomai.com

[R70] 时间戳与互转
来源：http://wet.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://xxy.birdmap.top

[R71] 日期格式化
来源：http://qmk.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://tho.fehbvm.com

[R72] 等待端口就绪
来源：http://iyv.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://gzw.chenjidiqi.icu

[R73] 分割大日志
来源：http://vdo.xuanzx.com

split -l 1000 big.log part_
来源：http://jwz.sweek.top

[R74] 批量重命名
来源：http://ubk.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wfp.ehwqpu.com

[R75] 导出环境变量
来源：http://ngc.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ycf.meibo888.top

[R76] 使用临时文件
来源：http://bcx.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nuy.hnxiangtu.top

[R77] 读取用户输入
来源：http://uog.gaohongyu789.top

read -rp "请输入: " ans
来源：http://ayd.sxryk.cn

[R78] 交互式菜单
来源：http://sta.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ygf.cheryme.top

[R79] 解析命令行选项
来源：http://awg.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hll.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://vjn.zdbjq.cn

time ./run.sh
来源：http://xej.tian-w.cn

================================================================================
来源：http://llt.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://zwn.ydjk.org.cn

================================================================================
来源：http://moe.smart0.xyz

[S01] C：Hello World
来源：http://ufj.cashguo.top

#include <stdio.h>
来源：http://pkz.sjlbkw.cn


<!-- 参考信息 -->