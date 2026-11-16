代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hgf.nanxinkj.top

) t WHERE rn = 1;
来源：http://bhc.daxiang520.top

[Q35] 内连接
来源：http://ucw.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xcj.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://ovi.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dnf.guowangkeji.top

[Q37] 右连接
来源：http://byy.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hgk.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cnc.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://emc.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://isj.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://aew.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ack.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oop.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kkg.feifeiyinyue.top

[Q41] 多表连接
来源：http://ksu.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://mgk.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://oar.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://gbj.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://bux.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://nze.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jcd.cdnleiting.top

[Q43] 标量子查询
来源：http://qge.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zxl.9152youxi.cn

[Q44] IN 子查询
来源：http://pbu.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://odx.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://mjt.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyn.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://qnx.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vny.xinyue.icu

[Q47] 与平均值比较
来源：http://uto.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ymg.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://euu.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qfu.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://vmn.tarul.cn

[Q49] 更新单行
来源：http://fie.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eox.sxryk.cn

[Q50] 批量更新
来源：http://qpb.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pqc.guowangkeji.top

[Q51] 用子查询更新
来源：http://lcm.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ubw.daxiang520.top

[Q52] 删除指定行
来源：http://ltu.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://mxc.pycfn.com

[Q53] 按条件删除
来源：http://lrc.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://msf.xylfe.cn

[Q54] 清空表
来源：http://kbn.wangdashe.top

TRUNCATE TABLE logs;
来源：http://fye.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://fra.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sqm.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://sxw.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qtv.birdmap.top

[Q57] 行号
来源：http://cfe.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wrd.zhixingplan.top

[Q58] 累计求和
来源：http://eok.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zep.sxryk.cn

[Q59] 分组内累计
来源：http://xyo.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pft.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://auu.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mwr.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxo.yanxiufei.cn

[Q61] 移动平均
来源：http://hql.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oyo.xylfe.cn

[Q62] 分组占比
来源：http://owk.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nsb.zhoulong.xyz

[Q63] 开启事务
来源：http://xkg.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://slc.zhixingplan.top

[Q64] 提交事务
来源：http://nyv.nanxinkj.top

COMMIT;
来源：http://djr.chenzaomai.com

[Q65] 回滚事务
来源：http://xdi.daria6918.cn

ROLLBACK;
来源：http://jea.birdmap.top

[Q66] 行锁查询
来源：http://cwm.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lvk.yj20258888.top

[Q67] 设置隔离级别
来源：http://txo.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ikv.xylfe.cn

[Q68] 保存点
来源：http://sur.c1oappe.top

SAVEPOINT sp1;
来源：http://hpe.daxiang520.top

ROLLBACK TO sp1;
来源：http://nmz.shzxlz.cn

[Q69] 查看执行计划
来源：http://mjd.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gya.mhx1999.top

[Q70] 更新统计信息
来源：http://wec.fehbvm.com

ANALYZE TABLE users;
来源：http://aqq.andypj.xyz

[Q71] 查看建表语句
来源：http://orl.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pkj.0kj1m.cn

[Q72] 查看索引
来源：http://nua.xziqi.cn

SHOW INDEX FROM users;
来源：http://usw.xziqi.cn

[Q73] 查看表状态
来源：http://bnu.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ycz.jqgfzy.top

[Q74] 强制使用索引
来源：http://jjb.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kov.birdmap.top

[Q75] 日期格式化
来源：http://rtf.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ymd.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://koi.yj20258.top

[Q76] 按天统计
来源：http://qxh.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://whr.ydzc1.top

[Q77] 时间加减
来源：http://mna.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sej.vqdsnc.cn

[Q78] 当前时间
来源：http://jwu.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bao.fengsongda.top

[Q79] 字符串拼接
来源：http://zwn.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://alz.0kj1m.cn

[Q80] 字符串截取
来源：http://vhx.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ddx.hysaishi.cn

[Q81] 字符串替换
来源：http://sup.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fbj.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://otu.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ief.iojbl.cn

[Q83] 大小写转换
来源：http://pqo.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyc.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://gnl.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://oav.guannengcc.top

[Q85] 数值取整
来源：http://vhv.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://npd.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://xra.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikv.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://vsn.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ali.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://tec.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gwr.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fgt.hammf.cn

[Q89] 判断表是否存在
来源：http://kyw.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ndf.andypj.xyz

[Q90] 生成序号列
来源：http://imo.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aih.chenlongwang.top

================================================================================
来源：http://bzw.zhiwuduotai.top

R. Bash 专题
来源：http://war.jinyuanbaomall.cn

================================================================================
来源：http://ekf.hammf.cn

[R01] shebang 与严格模式
来源：http://dkx.c1oappe.top

#!/usr/bin/env bash
来源：http://ptw.uphjek.com

set -euo pipefail
来源：http://xux.yuanzhike.top

[R02] 变量赋值与使用
来源：http://jmb.ivvv.top

name="Tom"; echo "$name"
来源：http://zvu.smart0.xyz

[R03] 只读变量
来源：http://ltk.xziqi.cn

readonly PI=3.14
来源：http://swy.shanyushiyangtech.top

[R04] 位置参数
来源：http://ogo.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vai.tarul.cn

[R05] 参数默认值
来源：http://byu.bjfxy.top

name="${1:-default}"
来源：http://dfo.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://nca.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://etx.yj20258888.top

[R07] if 判断文件
来源：http://skl.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nlr.xylfe.cn

[R08] 数值比较
来源：http://bis.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pxy.yfazqb.com

[R09] 字符串比较
来源：http://qgg.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://idx.hongshengwenyu.top

[R10] 正则匹配
来源：http://gdl.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rbh.0kj1m.cn

[R11] case 多分支
来源：http://jrr.xinyue.icu

case "$1" in
来源：http://mdt.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://ytk.dianchejie.cn

stop)  echo "停止" ;;
来源：http://fvm.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://vsa.jqgfzy.top

esac
来源：http://fgo.xziqi.cn

[R12] for 遍历文件
来源：http://qks.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://zbt.fktsv.cn

[R13] for 计数循环
来源：http://nck.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://aej.wangshuangyany.cn

[R14] C 风格 for
来源：http://abe.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://drf.mhx1999.top

[R15] while 逐行读文件
来源：http://kvd.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qtj.shzxlz.cn

[R16] until 等待条件
来源：http://djv.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://trs.xylfe.cn

[R17] 数组定义与取值
来源：http://iay.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uhy.havefunace.top

[R18] 遍历数组
来源：http://vhy.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gvs.mhx1999.top

[R19] 数组长度
来源：http://naa.aizwys.cn

echo "${#arr[@]}"
来源：http://hrm.redwolf501.top

[R20] 关联数组（字典）
来源：http://wyz.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kld.52xcode.cn

[R21] 字符串长度
来源：http://bjy.feifeiyinyue.top

echo "${#s}"
来源：http://azl.zdqjudy.top

[R22] 截取子串
来源：http://bio.sweek.top

echo "${s:0:5}"
来源：http://mvk.fktsv.cn

[R23] 字符串替换
来源：http://exl.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://myu.yueranfly.top

[R24] 大小写转换
来源：http://zku.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kjf.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://jwy.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zek.zdbjq.cn

[R26] 命令替换
来源：http://kog.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://kyf.sweek.top

[R27] 算术展开
来源：http://ehu.hammf.cn

echo $((1 + 2 * 3))
来源：http://wha.haohaochexian.top

[R28] 浮点运算
来源：http://esb.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://qlg.tian-w.cn

[R29] 定义函数
来源：http://grb.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gnh.0kj1m.cn

[R30] 函数返回状态码
来源：http://sar.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://gyj.vehdjk.com

[R31] 局部变量
来源：http://cth.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://bpg.zdbjq.cn

[R32] 参数个数校验
来源：http://qev.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dxj.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://xpy.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mdo.kuanghao11.cn

[R34] 退出时清理
来源：http://gtf.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://lay.yj20258.top

[R35] 后台执行并等待
来源：http://uki.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vnn.fzhhl.top

[R36] 并发执行多个任务
来源：http://vwp.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nrc.yuxming.cn

[R37] 把输出赋给变量
来源：http://qvu.cashguo.top

files=$(ls -1)
来源：http://xai.uphjek.com

[R38] 管道串联
来源：http://bza.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://tjz.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://hna.jqgufenzy.top

cmd > out.log 2>&1
来源：http://waw.wangdashe.top

[R40] 追加写日志
来源：http://ipo.birdmap.top

echo "log" >> out.log
来源：http://qkf.316326.xyz

[R41] 丢弃输出
来源：http://swy.gzhubu.top

cmd >/dev/null 2>&1
来源：http://swg.andypj.xyz

[R42] 输入重定向
来源：http://yat.fktsv.cn

wc -l < a.txt
来源：http://adf.meibo888.top

[R43] 按名字查找文件
来源：http://vik.zhijiandao.cn

find . -name "*.log" -type f
来源：http://myi.jianghu66.top

[R44] 按修改时间查找
来源：http://wpp.fengsongda.top

find . -mtime -7 -type f
来源：http://jtp.vqdsnc.cn

[R45] 批量删除
来源：http://tik.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://svm.chenlongwang.top

[R46] 递归替换文件内容
来源：http://yhx.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://msd.jqgfzy.top

[R47] sed 单行替换
来源：http://uvx.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zim.zhixingplan.top

[R48] awk 取指定列
来源：http://fvo.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://mtb.iojbl.cn

[R49] awk 带条件
来源：http://rsq.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bln.bbcook.cn

[R50] awk 求和
来源：http://teh.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://ife.ppjwa.cn

[R51] 排序去重取前几
来源：http://zmk.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://rvm.jiagoushi.top

[R52] 统计行数
来源：http://die.jlsjyb.cn

wc -l a.txt
来源：http://ybs.birdmap.top

[R53] 查看文件头与实时尾
来源：http://nzk.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fis.dashuyun.cn

[R54] 比较两个文件
来源：http://taf.52xcode.cn

diff a.txt b.txt
来源：http://uez.zhijiandao.cn

[R55] 压缩与解压
来源：http://czr.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pzv.quarkkingdee.top

[R56] 远程拷贝
来源：http://pmo.ydjk.org.cn

scp file user@host:/path/
来源：http://knu.andypj.xyz

[R57] 远程执行命令
来源：http://pty.cqqwz.cn

ssh user@host 'uptime'
来源：http://khx.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://obt.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xpl.316326.xyz

[R59] 发 POST JSON
来源：http://mbu.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sal.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://kqn.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gly.hongshengwenyu.top

[R61] 磁盘占用
来源：http://fyy.ctjpmb.com

df -h;  du -sh *
来源：http://lwu.xylfe.cn

[R62] 找最占空间的文件
来源：http://htw.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://tbn.fehbvm.com

[R63] 内存与进程
来源：http://dot.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://kvr.pycfn.com

[R64] 结束进程
来源：http://xcj.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://vjj.aibaodan.cn

[R65] 查看端口占用
来源：http://icy.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://skm.guowangkeji.top

[R66] 定时任务
来源：http://ozf.yuanzhike.top

crontab -e;  crontab -l
来源：http://pgt.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://vaz.yongpay.top

openssl rand -hex 16
来源：http://lah.yanxiufei.cn

[R68] 计算文件校验值
来源：http://qcs.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://gzv.hysaishi.cn

[R69] 生成随机密码
来源：http://pea.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://erd.52xcode.cn

[R70] 时间戳与互转
来源：http://ovi.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://gsf.ehwqpu.com

[R71] 日期格式化
来源：http://tjg.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eli.jlsjyb.cn

[R72] 等待端口就绪
来源：http://nmz.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ktf.52xcode.cn

[R73] 分割大日志
来源：http://mdt.jiagoushi.top

split -l 1000 big.log part_
来源：http://aus.yonumen.top

[R74] 批量重命名
来源：http://eai.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://agj.316326.xyz

[R75] 导出环境变量
来源：http://aiq.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://qks.gogol.net.cn

[R76] 使用临时文件
来源：http://gbv.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://two.jianghu66.top

[R77] 读取用户输入
来源：http://jpy.haohaochexian.top

read -rp "请输入: " ans
来源：http://oel.yj20258.top

[R78] 交互式菜单
来源：http://cjw.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kun.yueranfly.top

[R79] 解析命令行选项
来源：http://nsj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tdx.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://qun.yfazqb.com

time ./run.sh
来源：http://uha.tian-w.cn

================================================================================
来源：http://cog.ybcxt.top

S. C / C++ 专题
来源：http://smy.jiagoushi.top

================================================================================
来源：http://fvh.wangshuangyany.cn

[S01] C：Hello World
来源：http://ksi.yvedp.cn

#include <stdio.h>
来源：http://fgh.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tnk.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://lrs.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://ggi.yfazqb.com

[S03] C：读入整数
来源：http://fmu.yj20258888.top


<!-- 参考信息 -->