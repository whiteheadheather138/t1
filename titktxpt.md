代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://smu.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://zfc.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://soz.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yhs.ivvv.top

[Q33] 多列分组
来源：http://csz.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://brq.daxiang520.top

[Q34] 每组取第一条
来源：http://mdw.haohaochexian.top

SELECT * FROM (
来源：http://yqr.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kgv.gzhubu.top

) t WHERE rn = 1;
来源：http://eie.jlsjyb.cn

[Q35] 内连接
来源：http://glr.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://get.hywenlv.cn

[Q36] 左连接
来源：http://cvw.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ech.jinqigufen.top

[Q37] 右连接
来源：http://bni.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://owp.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://dnr.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mgi.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://qjr.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://dxj.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://exp.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://das.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://joi.jinghuilouyu.cn

[Q41] 多表连接
来源：http://gnf.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pua.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://whn.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://fdl.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://qki.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://rzk.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fvv.wangdashe.top

[Q43] 标量子查询
来源：http://egn.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pfs.daria6918.cn

[Q44] IN 子查询
来源：http://dkg.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jou.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://abc.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yew.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ruy.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lvu.pycfn.com

[Q47] 与平均值比较
来源：http://hke.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lnn.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://dvs.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nfg.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://taw.zhijiandao.cn

[Q49] 更新单行
来源：http://axh.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eex.zycfv.cn

[Q50] 批量更新
来源：http://czj.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ocy.jinqigufen.top

[Q51] 用子查询更新
来源：http://ctq.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xrm.hcnkem.com

[Q52] 删除指定行
来源：http://txe.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://szv.svipenyu.cn

[Q53] 按条件删除
来源：http://yor.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lbp.mhx1999.top

[Q54] 清空表
来源：http://hoj.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://ake.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://wpj.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ssf.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://uur.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ktp.aibaodan.cn

[Q57] 行号
来源：http://adb.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vdj.pengpengdd.cyou

[Q58] 累计求和
来源：http://stw.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pgh.redwolf501.top

[Q59] 分组内累计
来源：http://sug.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dkd.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://zff.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qpb.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fbq.hammf.cn

[Q61] 移动平均
来源：http://qhm.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://don.hnxiangtu.top

[Q62] 分组占比
来源：http://vzn.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uiz.zdbjq.cn

[Q63] 开启事务
来源：http://yev.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tnj.sufxvd.cn

[Q64] 提交事务
来源：http://drt.hcnkem.com

COMMIT;
来源：http://gaz.zycfv.cn

[Q65] 回滚事务
来源：http://wdp.tian-w.cn

ROLLBACK;
来源：http://bkz.yj20258888.top

[Q66] 行锁查询
来源：http://azx.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bgz.sweek.top

[Q67] 设置隔离级别
来源：http://nzh.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://emf.cqqwz.cn

[Q68] 保存点
来源：http://usq.guowangkeji.top

SAVEPOINT sp1;
来源：http://qin.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://avy.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://yoo.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://haj.yuanzhike.top

[Q70] 更新统计信息
来源：http://add.zycfv.cn

ANALYZE TABLE users;
来源：http://uai.nwbrower.top

[Q71] 查看建表语句
来源：http://bxu.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ywp.daxiang520.top

[Q72] 查看索引
来源：http://qsg.aibaodan.cn

SHOW INDEX FROM users;
来源：http://gtq.hnqzz.top

[Q73] 查看表状态
来源：http://jeh.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vig.jiagoushi.top

[Q74] 强制使用索引
来源：http://pgm.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uor.sysykeji.top

[Q75] 日期格式化
来源：http://xmx.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eac.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://czw.sufxvd.cn

[Q76] 按天统计
来源：http://xrq.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qtr.nwbrower.top

[Q77] 时间加减
来源：http://vxl.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tga.zdqjudy.top

[Q78] 当前时间
来源：http://iad.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tka.cheryme.top

[Q79] 字符串拼接
来源：http://uvv.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aqr.gogol.net.cn

[Q80] 字符串截取
来源：http://boi.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lqx.epnwcf.com

[Q81] 字符串替换
来源：http://vqc.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://avj.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://dlu.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gwu.guowangkeji.top

[Q83] 大小写转换
来源：http://uzx.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fix.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://sok.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://sse.sjlbkw.cn

[Q85] 数值取整
来源：http://yhk.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://knz.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://hgs.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hbr.birdmap.top

[Q87] JSON 字段做条件
来源：http://aud.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hae.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://vzg.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eah.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tqv.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://zmr.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rlk.gotoacloud.top

[Q90] 生成序号列
来源：http://epo.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oun.hfpthk.cn

================================================================================
来源：http://san.wangshuangyany.cn

R. Bash 专题
来源：http://eab.gogol.net.cn

================================================================================
来源：http://ybl.aibaodan.cn

[R01] shebang 与严格模式
来源：http://xpt.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://vwo.jinqigufen.top

set -euo pipefail
来源：http://uxh.meibo888.top

[R02] 变量赋值与使用
来源：http://xyx.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://qml.zhoulong.xyz

[R03] 只读变量
来源：http://fgs.yangfankeji.com

readonly PI=3.14
来源：http://xpw.kuanghao11.cn

[R04] 位置参数
来源：http://efz.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gwv.ivvv.top

[R05] 参数默认值
来源：http://cqj.hnqzz.top

name="${1:-default}"
来源：http://lkz.fktsv.cn

[R06] 判断命令是否存在
来源：http://pvf.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fsi.fanxiaobao.xyz

[R07] if 判断文件
来源：http://vin.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vdg.ppjwa.cn

[R08] 数值比较
来源：http://gwa.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cza.daria6918.cn

[R09] 字符串比较
来源：http://omm.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://orr.nanxinkj.top

[R10] 正则匹配
来源：http://nkm.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://emd.yongpay.top

[R11] case 多分支
来源：http://gmq.hnqzz.top

case "$1" in
来源：http://chx.gogol.net.cn

start) echo "启动" ;;
来源：http://lbz.yangfankeji.com

stop)  echo "停止" ;;
来源：http://msa.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://gpu.hesvh.cn

esac
来源：http://uex.guannengcc.top

[R12] for 遍历文件
来源：http://kdz.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://dzd.shzxlz.cn

[R13] for 计数循环
来源：http://afn.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://grv.birdmap.top

[R14] C 风格 for
来源：http://zdv.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rtt.nanxinkj.top

[R15] while 逐行读文件
来源：http://uzg.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mrs.guowangkeji.top

[R16] until 等待条件
来源：http://ulc.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dyo.zhijiandao.cn

[R17] 数组定义与取值
来源：http://vyp.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://pym.smart0.xyz

[R18] 遍历数组
来源：http://dqq.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uvi.jlsjyb.cn

[R19] 数组长度
来源：http://izt.c1oappe.top

echo "${#arr[@]}"
来源：http://xqq.daxiang520.top

[R20] 关联数组（字典）
来源：http://cab.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yvl.tian-w.cn

[R21] 字符串长度
来源：http://pmf.yanxiufei.cn

echo "${#s}"
来源：http://jry.uphjek.com

[R22] 截取子串
来源：http://xqh.ydjk.org.cn

echo "${s:0:5}"
来源：http://exq.wangshuangyany.cn

[R23] 字符串替换
来源：http://vxe.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hfd.zycfv.cn

[R24] 大小写转换
来源：http://hvr.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://dwj.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://lkq.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sqp.cdnleiting.top

[R26] 命令替换
来源：http://vkd.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://dos.hywenlv.cn

[R27] 算术展开
来源：http://vhb.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://qfl.daxiang520.top

[R28] 浮点运算
来源：http://qri.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://okt.jqgufenzy.top

[R29] 定义函数
来源：http://alj.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bfm.shuidangran.top

[R30] 函数返回状态码
来源：http://rlv.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://peu.0kj1m.cn

[R31] 局部变量
来源：http://efv.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://run.ctjpmb.com

[R32] 参数个数校验
来源：http://fap.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qkt.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://ufc.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://njx.gzhubu.top

[R34] 退出时清理
来源：http://jzc.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://zke.c1oappe.top

[R35] 后台执行并等待
来源：http://kfa.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dzz.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://kng.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jqi.daxiang520.top

[R37] 把输出赋给变量
来源：http://wmu.ybcxt.top

files=$(ls -1)
来源：http://zzl.sufxvd.cn

[R38] 管道串联
来源：http://dka.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://vms.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://cys.yuanzhike.top

cmd > out.log 2>&1
来源：http://owj.meibo888.top

[R40] 追加写日志
来源：http://ahw.ybcxt.top

echo "log" >> out.log
来源：http://sgr.gzhubu.top

[R41] 丢弃输出
来源：http://pqc.sweek.top

cmd >/dev/null 2>&1
来源：http://vaf.snrcjt.cn

[R42] 输入重定向
来源：http://zfz.mhx1999.top

wc -l < a.txt
来源：http://hco.yueranfly.top

[R43] 按名字查找文件
来源：http://wzi.jlsjyb.cn

find . -name "*.log" -type f
来源：http://cas.fzhhl.top

[R44] 按修改时间查找
来源：http://nof.gotoacloud.top

find . -mtime -7 -type f
来源：http://non.chenjidiqi.icu

[R45] 批量删除
来源：http://djc.sysykeji.top

find . -name "*.tmp" -delete
来源：http://cix.bjfxy.top

[R46] 递归替换文件内容
来源：http://fen.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jif.hnqzz.top

[R47] sed 单行替换
来源：http://ltu.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lag.tian-w.cn

[R48] awk 取指定列
来源：http://pad.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://vkf.yongpay.top

[R49] awk 带条件
来源：http://lmc.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://olj.sweek.top

[R50] awk 求和
来源：http://rmd.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bgi.ctjpmb.com

[R51] 排序去重取前几
来源：http://mmi.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sbu.bjfxy.top

[R52] 统计行数
来源：http://hdg.jinqigfzy.top

wc -l a.txt
来源：http://aqk.uphjek.com

[R53] 查看文件头与实时尾
来源：http://dod.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ciz.c1oappe.top

[R54] 比较两个文件
来源：http://jss.hnxiangtu.top

diff a.txt b.txt
来源：http://mmw.zdbjq.cn

[R55] 压缩与解压
来源：http://rvs.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qws.pengpengdd.cyou

[R56] 远程拷贝
来源：http://fam.fktsv.cn

scp file user@host:/path/
来源：http://jhn.zycfv.cn

[R57] 远程执行命令
来源：http://xwz.52xcode.cn

ssh user@host 'uptime'
来源：http://ywr.jiagoushi.top

[R58] 下载文件
来源：http://fwa.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ket.jianghu66.top

[R59] 发 POST JSON
来源：http://ihp.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mme.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://fhz.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ikh.cashguo.top

[R61] 磁盘占用
来源：http://tvn.haohaochexian.top

df -h;  du -sh *
来源：http://puz.cucudq.cn

[R62] 找最占空间的文件
来源：http://btf.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://xdb.zycfv.cn

[R63] 内存与进程
来源：http://jbw.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://elr.dianchejie.cn

[R64] 结束进程
来源：http://tgz.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://xzv.xziqi.cn

[R65] 查看端口占用
来源：http://fkn.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tdo.jqgufenzy.top

[R66] 定时任务
来源：http://cme.xziqi.cn

crontab -e;  crontab -l
来源：http://pst.yj20258888.top

[R67] 生成随机十六进制串
来源：http://zrc.jinqigufen.top

openssl rand -hex 16
来源：http://toj.ctjpmb.com

[R68] 计算文件校验值
来源：http://cua.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://mzo.jlsjyb.cn

[R69] 生成随机密码
来源：http://ikt.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://fds.tianlin.xyz

[R70] 时间戳与互转
来源：http://tmp.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://hbf.nanxuanxn.top

[R71] 日期格式化
来源：http://egn.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://glq.fzhhl.top

[R72] 等待端口就绪
来源：http://bwu.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://uoj.yfazqb.com

[R73] 分割大日志
来源：http://erh.chenlongwang.top

split -l 1000 big.log part_
来源：http://ota.shangyingyoupin.top

[R74] 批量重命名
来源：http://inn.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ryp.yuxming.cn

[R75] 导出环境变量
来源：http://fmi.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://iun.yanxiufei.cn

[R76] 使用临时文件
来源：http://pri.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pmn.ehwqpu.com

[R77] 读取用户输入
来源：http://rav.yongpay.top

read -rp "请输入: " ans
来源：http://obm.xziqi.cn

[R78] 交互式菜单
来源：http://ozc.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vgl.xinyue.icu

[R79] 解析命令行选项
来源：http://ked.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pte.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://irt.ybcxt.top

time ./run.sh
来源：http://vhx.xuetiantiany.cn

================================================================================
来源：http://ajp.tarul.cn


<!-- 参考信息 -->