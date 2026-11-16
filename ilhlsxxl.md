代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lky.jqgufenzy.top

) t WHERE rn = 1;
来源：http://wvx.zdbjq.cn

[Q35] 内连接
来源：http://myz.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rpg.xziqi.cn

[Q36] 左连接
来源：http://xuu.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zkg.epnwcf.com

[Q37] 右连接
来源：http://ygo.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qbm.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://qil.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xwt.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://wvc.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wyj.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dii.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aqh.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ehs.hcnkem.com

[Q41] 多表连接
来源：http://szu.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vxd.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://cij.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://hrb.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://ezn.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://zri.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fve.zdbjq.cn

[Q43] 标量子查询
来源：http://yrp.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zhp.dashuyun.cn

[Q44] IN 子查询
来源：http://gyy.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kbk.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://keu.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pie.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://isw.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hey.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://fyz.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ufx.havefunace.top

[Q48] CTE 公用表表达式
来源：http://fle.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://azh.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://ibc.nwbrower.top

[Q49] 更新单行
来源：http://rug.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://unw.yuanzhike.top

[Q50] 批量更新
来源：http://him.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cez.52xcode.cn

[Q51] 用子查询更新
来源：http://dah.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jjv.andypj.xyz

[Q52] 删除指定行
来源：http://zei.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://tce.zhongyouzk.top

[Q53] 按条件删除
来源：http://mbv.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dpu.yongpay.top

[Q54] 清空表
来源：http://ysa.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://ymk.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://qnt.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cpm.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://xhv.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://isq.ydjk.org.cn

[Q57] 行号
来源：http://ibh.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cvj.havefunace.top

[Q58] 累计求和
来源：http://qyb.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iys.tanke756.top

[Q59] 分组内累计
来源：http://mvb.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ycd.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://fpm.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kxp.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bjx.birdmap.top

[Q61] 移动平均
来源：http://ccv.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zas.jyoumei.cn

[Q62] 分组占比
来源：http://kjp.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://frv.zhiwuduotai.top

[Q63] 开启事务
来源：http://mxu.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ptj.guannengcc.top

[Q64] 提交事务
来源：http://ozz.yj20258888.top

COMMIT;
来源：http://hxn.ybcxt.top

[Q65] 回滚事务
来源：http://gbu.ydzc1.top

ROLLBACK;
来源：http://bpe.ctjpmb.com

[Q66] 行锁查询
来源：http://aab.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qtc.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://ckt.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vtp.meibo888.top

[Q68] 保存点
来源：http://ipd.bbcook.cn

SAVEPOINT sp1;
来源：http://szw.yj202588.top

ROLLBACK TO sp1;
来源：http://mly.kuanghao11.cn

[Q69] 查看执行计划
来源：http://epu.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ury.jqgfzy.top

[Q70] 更新统计信息
来源：http://ekb.xinyue.icu

ANALYZE TABLE users;
来源：http://gfw.vqdsnc.cn

[Q71] 查看建表语句
来源：http://spx.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://arp.ivvv.top

[Q72] 查看索引
来源：http://vnf.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://wye.sxryk.cn

[Q73] 查看表状态
来源：http://pqe.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ybk.c1oappe.top

[Q74] 强制使用索引
来源：http://bsg.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uts.dashuyun.cn

[Q75] 日期格式化
来源：http://iov.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ulj.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xej.zhoulong.xyz

[Q76] 按天统计
来源：http://rzt.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dig.gogol.net.cn

[Q77] 时间加减
来源：http://xbf.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mlx.zhoulong.xyz

[Q78] 当前时间
来源：http://tlg.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pqi.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://bpr.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ito.316326.xyz

[Q80] 字符串截取
来源：http://keo.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mmb.pengpengdd.cyou

[Q81] 字符串替换
来源：http://gya.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aju.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://ely.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rvz.hnqzz.top

[Q83] 大小写转换
来源：http://yqx.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kbv.yj20258888.top

[Q84] 去除首尾空格
来源：http://lov.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://jgd.yonumen.top

[Q85] 数值取整
来源：http://rwx.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ije.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://bav.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nnw.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://xen.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rcl.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://luq.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mij.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qog.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://bck.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://evj.yongpay.top

[Q90] 生成序号列
来源：http://tod.sysykeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tnz.gotoacloud.top

================================================================================
来源：http://ofm.gogol.net.cn

R. Bash 专题
来源：http://wbr.shuidangran.top

================================================================================
来源：http://rlw.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://xly.ybcxt.top

#!/usr/bin/env bash
来源：http://mbg.snrcjt.cn

set -euo pipefail
来源：http://juk.c1oappe.top

[R02] 变量赋值与使用
来源：http://nte.xuanzx.com

name="Tom"; echo "$name"
来源：http://bdf.yangfankeji.com

[R03] 只读变量
来源：http://blr.yj20258.top

readonly PI=3.14
来源：http://zqd.tarul.cn

[R04] 位置参数
来源：http://ahl.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kht.chenjidiqi.icu

[R05] 参数默认值
来源：http://gfs.hfpthk.cn

name="${1:-default}"
来源：http://idw.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://pog.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lji.hesvh.cn

[R07] if 判断文件
来源：http://chq.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://knj.zhiwuduotai.top

[R08] 数值比较
来源：http://npd.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ktw.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://kyt.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ada.zhongyouzk.top

[R10] 正则匹配
来源：http://arf.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://txg.fengsongda.top

[R11] case 多分支
来源：http://eja.quarkkingdee.top

case "$1" in
来源：http://wwh.hcnkem.com

start) echo "启动" ;;
来源：http://dif.uphjek.com

stop)  echo "停止" ;;
来源：http://htn.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://fwv.fanxiaobao.xyz

esac
来源：http://ciq.jqgufenzy.top

[R12] for 遍历文件
来源：http://zom.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://wfp.hongshengwenyu.top

[R13] for 计数循环
来源：http://zia.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://bbw.yfazqb.com

[R14] C 风格 for
来源：http://pqj.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ojy.zycfv.cn

[R15] while 逐行读文件
来源：http://sok.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uhm.daxiang520.top

[R16] until 等待条件
来源：http://uiw.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wcf.cdnleiting.top

[R17] 数组定义与取值
来源：http://zmg.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://yoo.wangshuangyany.cn

[R18] 遍历数组
来源：http://wlr.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tyi.bbcook.cn

[R19] 数组长度
来源：http://idh.yj202588.top

echo "${#arr[@]}"
来源：http://hne.yuanzhike.top

[R20] 关联数组（字典）
来源：http://zvz.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jbi.yj20258.top

[R21] 字符串长度
来源：http://fqd.redwolf501.top

echo "${#s}"
来源：http://pip.cucudq.cn

[R22] 截取子串
来源：http://vyf.9152youxi.cn

echo "${s:0:5}"
来源：http://xee.ehwqpu.com

[R23] 字符串替换
来源：http://rbm.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qal.yj20258.top

[R24] 大小写转换
来源：http://ruq.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://myt.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://uhq.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zzj.hcnkem.com

[R26] 命令替换
来源：http://wzf.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://bki.52xcode.cn

[R27] 算术展开
来源：http://xga.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://sea.zhengqikj.top

[R28] 浮点运算
来源：http://bnw.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://tra.svipenyu.cn

[R29] 定义函数
来源：http://fyr.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qht.yueranfly.top

[R30] 函数返回状态码
来源：http://xze.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://dwk.feifeiyinyue.top

[R31] 局部变量
来源：http://fnd.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://adu.hysaishi.cn

[R32] 参数个数校验
来源：http://ioi.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ihy.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://jpf.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://epi.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://okf.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rbd.tianlin.xyz

[R35] 后台执行并等待
来源：http://nda.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rqi.meibo888.top

[R36] 并发执行多个任务
来源：http://bnj.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://due.aizwys.cn

[R37] 把输出赋给变量
来源：http://xal.jlsjyb.cn

files=$(ls -1)
来源：http://hjy.fanxiaobao.xyz

[R38] 管道串联
来源：http://pko.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://qvp.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://yxv.bjfxy.top

cmd > out.log 2>&1
来源：http://txy.vqdsnc.cn

[R40] 追加写日志
来源：http://epn.chenjidiqi.icu

echo "log" >> out.log
来源：http://rwy.sufxvd.cn

[R41] 丢弃输出
来源：http://byy.yueranfly.top

cmd >/dev/null 2>&1
来源：http://dfr.havefunace.top

[R42] 输入重定向
来源：http://fsg.fzhhl.top

wc -l < a.txt
来源：http://wmm.bjfxy.top

[R43] 按名字查找文件
来源：http://rxq.cheryme.top

find . -name "*.log" -type f
来源：http://efy.yvedp.cn

[R44] 按修改时间查找
来源：http://apj.sweek.top

find . -mtime -7 -type f
来源：http://fvd.yueranfly.top

[R45] 批量删除
来源：http://ngq.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://zpy.cucudq.cn

[R46] 递归替换文件内容
来源：http://gbv.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://anq.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://ilz.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rzr.fktsv.cn

[R48] awk 取指定列
来源：http://wzm.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://ewt.yj20258888.top

[R49] awk 带条件
来源：http://xzn.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fys.yfazqb.com

[R50] awk 求和
来源：http://tlh.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://sor.nanxinkj.top

[R51] 排序去重取前几
来源：http://cxf.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ylg.ehwqpu.com

[R52] 统计行数
来源：http://ldg.svipenyu.cn

wc -l a.txt
来源：http://flc.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://jtn.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://unp.jiagoushi.top

[R54] 比较两个文件
来源：http://ody.chenzaomai.com

diff a.txt b.txt
来源：http://ukj.aibaodan.cn

[R55] 压缩与解压
来源：http://ugw.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eua.yuanzhike.top

[R56] 远程拷贝
来源：http://tzg.mhx1999.top

scp file user@host:/path/
来源：http://qhk.chenzaomai.com

[R57] 远程执行命令
来源：http://gbj.ppjwa.cn

ssh user@host 'uptime'
来源：http://yio.zhaomingkeji.xyz

[R58] 下载文件
来源：http://rqt.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rye.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://efb.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgq.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://inn.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ajr.fzhhl.top

[R61] 磁盘占用
来源：http://exp.hnxiangtu.top

df -h;  du -sh *
来源：http://hua.epnwcf.com

[R62] 找最占空间的文件
来源：http://wvi.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://ano.hnxiangtu.top

[R63] 内存与进程
来源：http://mrd.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://daz.yj20258888.top

[R64] 结束进程
来源：http://roy.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://ual.meibo888.top

[R65] 查看端口占用
来源：http://uar.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pdc.hcnkem.com

[R66] 定时任务
来源：http://fun.yj202588.top

crontab -e;  crontab -l
来源：http://odk.xziqi.cn

[R67] 生成随机十六进制串
来源：http://dme.shangyingyoupin.top

openssl rand -hex 16
来源：http://pmq.mhx1999.top

[R68] 计算文件校验值
来源：http://can.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://esm.yj20258.top

[R69] 生成随机密码
来源：http://yen.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://puw.fengsongda.top

[R70] 时间戳与互转
来源：http://nih.vehdjk.com

date +%s;  date -d @1700000000
来源：http://umv.yangfankeji.com

[R71] 日期格式化
来源：http://mpj.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zgm.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://llw.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hqx.kuanghao11.cn

[R73] 分割大日志
来源：http://tiu.jiagoushi.top

split -l 1000 big.log part_
来源：http://dyp.gogol.net.cn

[R74] 批量重命名
来源：http://usf.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://csb.snrcjt.cn

[R75] 导出环境变量
来源：http://bvh.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://ehk.jinqigfzy.top

[R76] 使用临时文件
来源：http://kpq.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://axp.gotoacloud.top

[R77] 读取用户输入
来源：http://fcb.zhixingplan.top

read -rp "请输入: " ans
来源：http://fri.daria6918.cn

[R78] 交互式菜单
来源：http://eyh.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rlg.yanxiufei.cn

[R79] 解析命令行选项
来源：http://uxg.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iik.cheryme.top

[R80] 查看脚本执行耗时
来源：http://hys.chenzaomai.com

time ./run.sh
来源：http://vmg.yj20258.top

================================================================================
来源：http://xou.pycfn.com

S. C / C++ 专题
来源：http://vnl.sysykeji.top

================================================================================
来源：http://uhf.0kj1m.cn

[S01] C：Hello World
来源：http://cwx.xziqi.cn

#include <stdio.h>
来源：http://rkk.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://smi.redwolf501.top

[S02] C：变量与格式化输出
来源：http://fve.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://rad.vehdjk.com

[S03] C：读入整数
来源：http://ymt.jinyuanbaomall.cn


<!-- 参考信息 -->