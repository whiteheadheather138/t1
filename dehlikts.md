代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pnr.chenlongwang.top

) t WHERE rn = 1;
来源：http://emm.hcnkem.com

[Q35] 内连接
来源：http://ezg.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yly.vehdjk.com

[Q36] 左连接
来源：http://gce.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aqt.zdbjq.cn

[Q37] 右连接
来源：http://oin.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ppr.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://orr.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opl.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://jux.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iso.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jkr.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://upr.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zwg.zhixingplan.top

[Q41] 多表连接
来源：http://krc.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gaw.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://hye.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://uoh.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://lib.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://plc.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hrn.yuxming.cn

[Q43] 标量子查询
来源：http://lam.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ecg.yangfankeji.com

[Q44] IN 子查询
来源：http://dah.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rxf.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://obd.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jtb.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://vjc.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kng.quarkkingdee.top

[Q47] 与平均值比较
来源：http://mgo.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fuk.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://via.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xvg.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://ypo.yfazqb.com

[Q49] 更新单行
来源：http://cvv.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fry.zycfv.cn

[Q50] 批量更新
来源：http://dlk.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qbo.uphjek.com

[Q51] 用子查询更新
来源：http://vie.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://inf.nanxuanxn.top

[Q52] 删除指定行
来源：http://ron.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://tlt.svipenyu.cn

[Q53] 按条件删除
来源：http://snz.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qhl.havefunace.top

[Q54] 清空表
来源：http://fnj.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://fwg.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://tek.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bda.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://thq.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ynm.jyoumei.cn

[Q57] 行号
来源：http://bit.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yuk.yj20258.top

[Q58] 累计求和
来源：http://uqz.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hec.yonumen.top

[Q59] 分组内累计
来源：http://gji.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://syh.sweek.top

[Q60] 取上一行 / 下一行
来源：http://zou.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tuo.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pnx.nanxinkj.top

[Q61] 移动平均
来源：http://gou.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qea.guowangkeji.top

[Q62] 分组占比
来源：http://xpj.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yie.yj202588.top

[Q63] 开启事务
来源：http://gkm.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aqh.ppjwa.cn

[Q64] 提交事务
来源：http://rwr.ywan-chungtsiang.top

COMMIT;
来源：http://zzl.yj20258888.top

[Q65] 回滚事务
来源：http://rgg.feifeiyinyue.top

ROLLBACK;
来源：http://wvz.yueranfly.top

[Q66] 行锁查询
来源：http://upo.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vvp.yfazqb.com

[Q67] 设置隔离级别
来源：http://twn.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eji.hywenlv.cn

[Q68] 保存点
来源：http://iiy.daxiang520.top

SAVEPOINT sp1;
来源：http://qtn.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://rrx.yuanzhike.top

[Q69] 查看执行计划
来源：http://ylk.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pjy.yongpay.top

[Q70] 更新统计信息
来源：http://hrk.birdmap.top

ANALYZE TABLE users;
来源：http://tcw.fehbvm.com

[Q71] 查看建表语句
来源：http://nua.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vcd.yongpay.top

[Q72] 查看索引
来源：http://bzy.gogol.net.cn

SHOW INDEX FROM users;
来源：http://pdm.zdqjudy.top

[Q73] 查看表状态
来源：http://ayl.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hbh.yonumen.top

[Q74] 强制使用索引
来源：http://wlo.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lif.hnxiangtu.top

[Q75] 日期格式化
来源：http://kor.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jwx.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xgl.guannengcc.top

[Q76] 按天统计
来源：http://bal.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pfl.daxiang520.top

[Q77] 时间加减
来源：http://yrp.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fbt.sysykeji.top

[Q78] 当前时间
来源：http://ccb.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qri.meibo888.top

[Q79] 字符串拼接
来源：http://znh.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jop.chenzaomai.com

[Q80] 字符串截取
来源：http://klz.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gff.fengsongda.top

[Q81] 字符串替换
来源：http://itw.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sor.hammf.cn

[Q82] 字符长度与字节长度
来源：http://psm.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ada.ydjk.org.cn

[Q83] 大小写转换
来源：http://wdw.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lwg.shzxlz.cn

[Q84] 去除首尾空格
来源：http://lmt.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://iid.xinyue.icu

[Q85] 数值取整
来源：http://klg.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://owi.uphjek.com

[Q86] 读取 JSON 字段
来源：http://etd.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://smf.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://jhc.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kmf.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://rdp.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://svu.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lfm.zycfv.cn

[Q89] 判断表是否存在
来源：http://ynp.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dkr.mhx1999.top

[Q90] 生成序号列
来源：http://lzs.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://obi.316326.xyz

================================================================================
来源：http://ebg.c1oappe.top

R. Bash 专题
来源：http://qlk.zhengqikj.top

================================================================================
来源：http://mra.ybcxt.top

[R01] shebang 与严格模式
来源：http://hzc.sufxvd.cn

#!/usr/bin/env bash
来源：http://uyh.bbcook.cn

set -euo pipefail
来源：http://ghn.fehbvm.com

[R02] 变量赋值与使用
来源：http://wds.zhengqikj.top

name="Tom"; echo "$name"
来源：http://dgb.yj202588.top

[R03] 只读变量
来源：http://nwg.gotoacloud.top

readonly PI=3.14
来源：http://rym.meibo888.top

[R04] 位置参数
来源：http://wvg.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sxb.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://niz.hammf.cn

name="${1:-default}"
来源：http://yvi.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://gmw.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://scd.yj20258.top

[R07] if 判断文件
来源：http://yua.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cmr.ydzc1.top

[R08] 数值比较
来源：http://jfm.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://mkn.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://dwk.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qws.gaohongyu789.top

[R10] 正则匹配
来源：http://ctv.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://prw.bjfxy.top

[R11] case 多分支
来源：http://tlz.feifeiyinyue.top

case "$1" in
来源：http://osk.316326.xyz

start) echo "启动" ;;
来源：http://lgv.jinqigufen.top

stop)  echo "停止" ;;
来源：http://rao.tanke756.top

*)     echo "未知命令" ;;
来源：http://pqn.hcnkem.com

esac
来源：http://bjz.chenjidiqi.icu

[R12] for 遍历文件
来源：http://aah.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://wgv.uphjek.com

[R13] for 计数循环
来源：http://nfd.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://quo.jqgufenzy.top

[R14] C 风格 for
来源：http://ehu.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hxs.xuanzx.com

[R15] while 逐行读文件
来源：http://rzh.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hvp.epnwcf.com

[R16] until 等待条件
来源：http://uah.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ikb.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://vrk.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://yjt.fanxiaobao.xyz

[R18] 遍历数组
来源：http://dnu.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sjh.yanxiufei.cn

[R19] 数组长度
来源：http://yfs.quarkkingdee.top

echo "${#arr[@]}"
来源：http://gkr.xinyue.icu

[R20] 关联数组（字典）
来源：http://zns.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://egp.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://tnk.tianlin.xyz

echo "${#s}"
来源：http://mre.cheryme.top

[R22] 截取子串
来源：http://kqj.vqdsnc.cn

echo "${s:0:5}"
来源：http://xkg.pengpengdd.cyou

[R23] 字符串替换
来源：http://qli.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vhs.quarkkingdee.top

[R24] 大小写转换
来源：http://pyc.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wwf.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://pet.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tob.shuidangran.top

[R26] 命令替换
来源：http://zzo.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://moo.jinqigfzy.top

[R27] 算术展开
来源：http://jhu.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://eag.xuanzx.com

[R28] 浮点运算
来源：http://jrp.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://orl.dashuyun.cn

[R29] 定义函数
来源：http://hoi.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xyu.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://vtm.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://kfw.fengsongda.top

[R31] 局部变量
来源：http://wxo.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://lej.cqqwz.cn

[R32] 参数个数校验
来源：http://hlh.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kvh.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://eyg.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jqj.ydzc1.top

[R34] 退出时清理
来源：http://hwj.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://qnn.snrcjt.cn

[R35] 后台执行并等待
来源：http://tly.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mmn.yj20258888.top

[R36] 并发执行多个任务
来源：http://cik.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hib.tanke756.top

[R37] 把输出赋给变量
来源：http://qpc.yueranfly.top

files=$(ls -1)
来源：http://oaa.daxiang520.top

[R38] 管道串联
来源：http://fhv.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://ivq.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://qda.yueranfly.top

cmd > out.log 2>&1
来源：http://fdo.hesvh.cn

[R40] 追加写日志
来源：http://sep.vehdjk.com

echo "log" >> out.log
来源：http://uhz.tarul.cn

[R41] 丢弃输出
来源：http://qde.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://scm.sysykeji.top

[R42] 输入重定向
来源：http://wgo.xziqi.cn

wc -l < a.txt
来源：http://jhr.hcnkem.com

[R43] 按名字查找文件
来源：http://exn.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://bfc.birdmap.top

[R44] 按修改时间查找
来源：http://qgg.jinqigfzy.top

find . -mtime -7 -type f
来源：http://ktw.havefunace.top

[R45] 批量删除
来源：http://hvi.sxryk.cn

find . -name "*.tmp" -delete
来源：http://hyj.yvedp.cn

[R46] 递归替换文件内容
来源：http://lgj.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lgs.tanke756.top

[R47] sed 单行替换
来源：http://sff.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://nvo.cashguo.top

[R48] awk 取指定列
来源：http://auw.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://kmm.tian-w.cn

[R49] awk 带条件
来源：http://vno.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ztx.feifeiyinyue.top

[R50] awk 求和
来源：http://aox.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sjy.hfpthk.cn

[R51] 排序去重取前几
来源：http://mpl.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hxe.ybcxt.top

[R52] 统计行数
来源：http://qjz.tianlin.xyz

wc -l a.txt
来源：http://yun.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://sxn.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lar.meibo888.top

[R54] 比较两个文件
来源：http://wcg.quarkkingdee.top

diff a.txt b.txt
来源：http://jwl.yuanzhike.top

[R55] 压缩与解压
来源：http://myc.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jev.vehdjk.com

[R56] 远程拷贝
来源：http://oaq.ybcxt.top

scp file user@host:/path/
来源：http://zku.vqdsnc.cn

[R57] 远程执行命令
来源：http://paf.zhijiandao.cn

ssh user@host 'uptime'
来源：http://yld.hammf.cn

[R58] 下载文件
来源：http://itr.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://awg.shuidangran.top

[R59] 发 POST JSON
来源：http://cfb.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://riu.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://nwx.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ewe.sxryk.cn

[R61] 磁盘占用
来源：http://erm.yj20258.top

df -h;  du -sh *
来源：http://auv.redwolf501.top

[R62] 找最占空间的文件
来源：http://sqm.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://eql.birdmap.top

[R63] 内存与进程
来源：http://owj.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://muu.cucudq.cn

[R64] 结束进程
来源：http://qpr.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://dok.svipenyu.cn

[R65] 查看端口占用
来源：http://lpn.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xwp.hongshengwenyu.top

[R66] 定时任务
来源：http://wsr.havefunace.top

crontab -e;  crontab -l
来源：http://yec.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://afi.hongshengwenyu.top

openssl rand -hex 16
来源：http://tur.birdmap.top

[R68] 计算文件校验值
来源：http://lwt.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://nvl.yj20258888.top

[R69] 生成随机密码
来源：http://zdu.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://vpk.cqqwz.cn

[R70] 时间戳与互转
来源：http://wfe.zycfv.cn

date +%s;  date -d @1700000000
来源：http://nmo.yfazqb.com

[R71] 日期格式化
来源：http://znc.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://uot.jinqigufen.top

[R72] 等待端口就绪
来源：http://gfl.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lgn.svipenyu.cn

[R73] 分割大日志
来源：http://drd.xinyue.icu

split -l 1000 big.log part_
来源：http://brb.ybcxt.top

[R74] 批量重命名
来源：http://gnf.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nqz.xziqi.cn

[R75] 导出环境变量
来源：http://vbr.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://ump.guowangkeji.top

[R76] 使用临时文件
来源：http://txu.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tdu.gzhubu.top

[R77] 读取用户输入
来源：http://tve.yj20258888.top

read -rp "请输入: " ans
来源：http://sgz.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://gnz.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://aec.0kj1m.cn

[R79] 解析命令行选项
来源：http://pfi.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mxh.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://dhh.shuidangran.top

time ./run.sh
来源：http://txa.havefunace.top

================================================================================
来源：http://wod.mhx1999.top

S. C / C++ 专题
来源：http://dgb.hesvh.cn

================================================================================
来源：http://ufi.xuetiantiany.cn

[S01] C：Hello World
来源：http://mdt.hnqzz.top

#include <stdio.h>
来源：http://krt.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yvh.fzhhl.top

[S02] C：变量与格式化输出
来源：http://ymi.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://pem.xinyue.icu

[S03] C：读入整数
来源：http://dom.shuidangran.top


<!-- 参考信息 -->