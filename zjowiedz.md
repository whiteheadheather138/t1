代发 wailian999

[Q36] 左连接
来源：http://nox.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jyy.cucudq.cn

[Q37] 右连接
来源：http://qrm.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ayb.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://nig.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xay.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://coh.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ttt.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mum.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uex.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bpz.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://faf.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dui.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://boi.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ueu.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://cda.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://mjk.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whv.xinyue.icu

[Q43] 标量子查询
来源：http://kke.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dso.yuanzhike.top

[Q44] IN 子查询
来源：http://pbl.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tjf.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://ydc.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bif.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://kir.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmq.yangfankeji.com

[Q47] 与平均值比较
来源：http://dyl.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vqb.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://pni.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qco.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://det.birdmap.top

[Q49] 更新单行
来源：http://wgx.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.fengsongda.top

[Q50] 批量更新
来源：http://rpt.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iie.c1oappe.top

[Q51] 用子查询更新
来源：http://sxm.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lny.jinqigfzy.top

[Q52] 删除指定行
来源：http://wha.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://jze.quarkkingdee.top

[Q53] 按条件删除
来源：http://ndt.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fwj.zdbjq.cn

[Q54] 清空表
来源：http://ods.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://xiq.mhx1999.top

[Q55] 排名（并列占位）
来源：http://ygq.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zdk.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://wlx.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zhn.shzxlz.cn

[Q57] 行号
来源：http://xff.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tyn.jinghuilouyu.cn

[Q58] 累计求和
来源：http://asp.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixi.gogol.net.cn

[Q59] 分组内累计
来源：http://srw.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kur.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://orb.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://axx.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sge.c1oappe.top

[Q61] 移动平均
来源：http://quj.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lhd.guowangkeji.top

[Q62] 分组占比
来源：http://zdp.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hmy.daxiang520.top

[Q63] 开启事务
来源：http://caw.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://syw.svipenyu.cn

[Q64] 提交事务
来源：http://lvm.gogol.net.cn

COMMIT;
来源：http://era.chenlongwang.top

[Q65] 回滚事务
来源：http://por.sweek.top

ROLLBACK;
来源：http://zdg.yuanzhike.top

[Q66] 行锁查询
来源：http://mkt.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ief.shzxlz.cn

[Q67] 设置隔离级别
来源：http://brf.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncz.yanxiufei.cn

[Q68] 保存点
来源：http://adf.hesvh.cn

SAVEPOINT sp1;
来源：http://gjj.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://feh.cashguo.top

[Q69] 查看执行计划
来源：http://ove.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hnd.hcnkem.com

[Q70] 更新统计信息
来源：http://tiw.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://nou.daxiang520.top

[Q71] 查看建表语句
来源：http://zlw.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ljo.cheryme.top

[Q72] 查看索引
来源：http://kyp.jianghu66.top

SHOW INDEX FROM users;
来源：http://zej.redwolf501.top

[Q73] 查看表状态
来源：http://vlm.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tat.snrcjt.cn

[Q74] 强制使用索引
来源：http://mwr.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rad.sysykeji.top

[Q75] 日期格式化
来源：http://krd.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uja.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pmb.hesvh.cn

[Q76] 按天统计
来源：http://lbq.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ool.jyoumei.cn

[Q77] 时间加减
来源：http://vds.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kax.pengpengdd.cyou

[Q78] 当前时间
来源：http://xdf.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wof.daxiang520.top

[Q79] 字符串拼接
来源：http://xhz.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vcv.bbcook.cn

[Q80] 字符串截取
来源：http://ggs.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dkr.ivvv.top

[Q81] 字符串替换
来源：http://fux.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://haf.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://vub.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://osm.daria6918.cn

[Q83] 大小写转换
来源：http://xnn.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tmm.haohaochexian.top

[Q84] 去除首尾空格
来源：http://tjm.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://kwj.yonumen.top

[Q85] 数值取整
来源：http://ueg.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bbe.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://czc.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mlo.epnwcf.com

[Q87] JSON 字段做条件
来源：http://zcf.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fbt.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://cls.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vhc.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kgk.zhengqikj.top

[Q89] 判断表是否存在
来源：http://any.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jtz.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://kdt.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zir.havefunace.top

================================================================================
来源：http://zqb.pycfn.com

R. Bash 专题
来源：http://tve.gaohongyu789.top

================================================================================
来源：http://ubs.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://hgz.hnxiangtu.top

#!/usr/bin/env bash
来源：http://wsb.shangyingyoupin.top

set -euo pipefail
来源：http://ynv.c1oappe.top

[R02] 变量赋值与使用
来源：http://yri.tarul.cn

name="Tom"; echo "$name"
来源：http://pco.jyoumei.cn

[R03] 只读变量
来源：http://uoz.guannengcc.top

readonly PI=3.14
来源：http://gij.tanke756.top

[R04] 位置参数
来源：http://bwo.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fcs.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://byn.xuetiantiany.cn

name="${1:-default}"
来源：http://wpw.yvedp.cn

[R06] 判断命令是否存在
来源：http://wsc.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sqh.52xcode.cn

[R07] if 判断文件
来源：http://dpz.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ula.jlsjyb.cn

[R08] 数值比较
来源：http://pch.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://udp.hesvh.cn

[R09] 字符串比较
来源：http://ydq.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pat.ybcxt.top

[R10] 正则匹配
来源：http://rhm.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jyh.hnxiangtu.top

[R11] case 多分支
来源：http://nrh.yuanzhike.top

case "$1" in
来源：http://nlq.hammf.cn

start) echo "启动" ;;
来源：http://hie.gogol.net.cn

stop)  echo "停止" ;;
来源：http://nrm.vehdjk.com

*)     echo "未知命令" ;;
来源：http://eoo.hammf.cn

esac
来源：http://epx.yj20258.top

[R12] for 遍历文件
来源：http://mzc.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://snd.316326.xyz

[R13] for 计数循环
来源：http://doj.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://koe.haohaochexian.top

[R14] C 风格 for
来源：http://yvg.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qfb.fktsv.cn

[R15] while 逐行读文件
来源：http://len.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nkz.sxryk.cn

[R16] until 等待条件
来源：http://svh.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://haq.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://abj.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://yxf.quarkkingdee.top

[R18] 遍历数组
来源：http://giy.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://afm.tianlin.xyz

[R19] 数组长度
来源：http://qwf.ydzc1.top

echo "${#arr[@]}"
来源：http://vnh.jyoumei.cn

[R20] 关联数组（字典）
来源：http://qzc.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xcj.feifeiyinyue.top

[R21] 字符串长度
来源：http://cby.zdqjudy.top

echo "${#s}"
来源：http://nia.smart0.xyz

[R22] 截取子串
来源：http://oxf.wangdashe.top

echo "${s:0:5}"
来源：http://rtm.jqgfzy.top

[R23] 字符串替换
来源：http://mir.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sgp.yuxming.cn

[R24] 大小写转换
来源：http://eec.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://eeo.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://gdj.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kkw.tianlin.xyz

[R26] 命令替换
来源：http://mrz.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://oao.sxryk.cn

[R27] 算术展开
来源：http://tgu.yongpay.top

echo $((1 + 2 * 3))
来源：http://neb.zhijiandao.cn

[R28] 浮点运算
来源：http://crh.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://zgs.daria6918.cn

[R29] 定义函数
来源：http://kjq.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://goj.sjlbkw.cn

[R30] 函数返回状态码
来源：http://eox.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://lcr.iojbl.cn

[R31] 局部变量
来源：http://aea.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://kpe.0kj1m.cn

[R32] 参数个数校验
来源：http://fct.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yqs.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://pma.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://llv.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://fwy.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://rjv.jyoumei.cn

[R35] 后台执行并等待
来源：http://ant.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://liz.zhengqikj.top

[R36] 并发执行多个任务
来源：http://izw.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://edn.guowangkeji.top

[R37] 把输出赋给变量
来源：http://pax.zycfv.cn

files=$(ls -1)
来源：http://zqt.tanke756.top

[R38] 管道串联
来源：http://cog.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://frr.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://dao.uphjek.com

cmd > out.log 2>&1
来源：http://jbb.mhx1999.top

[R40] 追加写日志
来源：http://txl.mhx1999.top

echo "log" >> out.log
来源：http://pdp.svipenyu.cn

[R41] 丢弃输出
来源：http://vyj.gzhubu.top

cmd >/dev/null 2>&1
来源：http://qns.zhiwuduotai.top

[R42] 输入重定向
来源：http://cjt.smart0.xyz

wc -l < a.txt
来源：http://ixc.bjfxy.top

[R43] 按名字查找文件
来源：http://ehw.chenzaomai.com

find . -name "*.log" -type f
来源：http://zsz.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://jlb.yuanzhike.top

find . -mtime -7 -type f
来源：http://prw.jianghu66.top

[R45] 批量删除
来源：http://pja.havefunace.top

find . -name "*.tmp" -delete
来源：http://xcu.guannengcc.top

[R46] 递归替换文件内容
来源：http://krh.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cqi.smart0.xyz

[R47] sed 单行替换
来源：http://nzo.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://kub.sjlbkw.cn

[R48] awk 取指定列
来源：http://khy.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://dcz.xuanzx.com

[R49] awk 带条件
来源：http://qsz.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://myb.hongshengwenyu.top

[R50] awk 求和
来源：http://btq.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://iup.hammf.cn

[R51] 排序去重取前几
来源：http://lnv.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nfn.jlsjyb.cn

[R52] 统计行数
来源：http://ilm.nwbrower.top

wc -l a.txt
来源：http://wao.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://fuh.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xun.hfpthk.cn

[R54] 比较两个文件
来源：http://xzv.daria6918.cn

diff a.txt b.txt
来源：http://tlz.hnqzz.top

[R55] 压缩与解压
来源：http://rkt.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nfc.cqqwz.cn

[R56] 远程拷贝
来源：http://ewv.xinyue.icu

scp file user@host:/path/
来源：http://iwz.hesvh.cn

[R57] 远程执行命令
来源：http://vpc.kuanghao11.cn

ssh user@host 'uptime'
来源：http://nik.ywan-chungtsiang.top

[R58] 下载文件
来源：http://beg.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ipk.gzhubu.top

[R59] 发 POST JSON
来源：http://thn.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ndz.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://zrg.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jdc.yongpay.top

[R61] 磁盘占用
来源：http://adp.hnqzz.top

df -h;  du -sh *
来源：http://foi.hnqzz.top

[R62] 找最占空间的文件
来源：http://fus.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://xis.hcnkem.com

[R63] 内存与进程
来源：http://oug.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://qkh.zhoulong.xyz

[R64] 结束进程
来源：http://syj.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://jhn.9152youxi.cn

[R65] 查看端口占用
来源：http://dcb.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pnw.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://mls.yanxiufei.cn

crontab -e;  crontab -l
来源：http://whz.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://pqn.sufxvd.cn

openssl rand -hex 16
来源：http://shu.aibaodan.cn

[R68] 计算文件校验值
来源：http://fqs.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://exx.sxryk.cn

[R69] 生成随机密码
来源：http://yjh.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://lsl.nanxuanxn.top

[R70] 时间戳与互转
来源：http://ibo.pycfn.com

date +%s;  date -d @1700000000
来源：http://rhc.zdqjudy.top

[R71] 日期格式化
来源：http://stw.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://joj.kuanghao11.cn

[R72] 等待端口就绪
来源：http://jhm.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://myd.gzhubu.top

[R73] 分割大日志
来源：http://ghw.tian-w.cn

split -l 1000 big.log part_
来源：http://sfd.cheryme.top

[R74] 批量重命名
来源：http://hnn.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dlq.yvedp.cn

[R75] 导出环境变量
来源：http://qzv.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://vjs.haohaochexian.top

[R76] 使用临时文件
来源：http://wsf.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rwy.chenlongwang.top

[R77] 读取用户输入
来源：http://esx.uphjek.com

read -rp "请输入: " ans
来源：http://ldi.jinqigfzy.top

[R78] 交互式菜单
来源：http://jip.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wtf.yj202588.top

[R79] 解析命令行选项
来源：http://dpw.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tvo.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://nuq.yj202588.top

time ./run.sh
来源：http://hry.xinyue.icu

================================================================================
来源：http://ime.jyoumei.cn

S. C / C++ 专题
来源：http://zbp.sufxvd.cn

================================================================================
来源：http://ksj.guowangkeji.top

[S01] C：Hello World
来源：http://hqx.zhiwuduotai.top

#include <stdio.h>
来源：http://cal.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://orb.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://fed.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://qsg.guannengcc.top

[S03] C：读入整数
来源：http://zls.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://qel.havefunace.top

[S04] C：字符串复制
来源：http://mhf.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://rlr.dashuyun.cn

[S05] C：字符串长度
来源：http://dwp.jianghu66.top


<!-- 参考信息 -->