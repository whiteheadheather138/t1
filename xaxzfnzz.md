代发 wailian999

[Q33] 多列分组
来源：http://ysu.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ape.hammf.cn

[Q34] 每组取第一条
来源：http://llq.aibaodan.cn

SELECT * FROM (
来源：http://izt.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://heh.zhengqikj.top

) t WHERE rn = 1;
来源：http://sin.fktsv.cn

[Q35] 内连接
来源：http://mwd.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gdu.sysykeji.top

[Q36] 左连接
来源：http://ezt.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwk.redwolf501.top

[Q37] 右连接
来源：http://obn.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sez.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://swh.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mdd.havefunace.top

[Q39] 自连接（查上下级）
来源：http://psu.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://brl.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uat.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dsm.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://koh.hywenlv.cn

[Q41] 多表连接
来源：http://cfb.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hoh.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://tua.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://lmg.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://zhc.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://eef.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uom.daria6918.cn

[Q43] 标量子查询
来源：http://qiq.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cej.dianchejie.cn

[Q44] IN 子查询
来源：http://hij.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zij.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://hmy.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lzz.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://zdd.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tws.wangdashe.top

[Q47] 与平均值比较
来源：http://yar.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://frn.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://adw.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xgq.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://jwo.kuanghao11.cn

[Q49] 更新单行
来源：http://mba.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bxu.zycfv.cn

[Q50] 批量更新
来源：http://ntd.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aou.xinyue.icu

[Q51] 用子查询更新
来源：http://for.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://syj.aizwys.cn

[Q52] 删除指定行
来源：http://oip.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://eog.shuidangran.top

[Q53] 按条件删除
来源：http://pya.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gqc.chenlongwang.top

[Q54] 清空表
来源：http://lsv.bjfxy.top

TRUNCATE TABLE logs;
来源：http://kpk.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://lhr.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vqc.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://nqn.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvz.chenzaomai.com

[Q57] 行号
来源：http://jnt.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jsm.redwolf501.top

[Q58] 累计求和
来源：http://fys.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://low.daria6918.cn

[Q59] 分组内累计
来源：http://gls.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mzz.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://iiv.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ntr.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nhq.iojbl.cn

[Q61] 移动平均
来源：http://xdi.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eww.316326.xyz

[Q62] 分组占比
来源：http://evl.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xrm.xinyue.icu

[Q63] 开启事务
来源：http://uup.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://muz.ppjwa.cn

[Q64] 提交事务
来源：http://mqk.yj202588.top

COMMIT;
来源：http://mci.cucudq.cn

[Q65] 回滚事务
来源：http://erg.fzhhl.top

ROLLBACK;
来源：http://gzi.svipenyu.cn

[Q66] 行锁查询
来源：http://cem.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nvc.fengsongda.top

[Q67] 设置隔离级别
来源：http://ioo.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zmw.andypj.xyz

[Q68] 保存点
来源：http://iid.yuanzhike.top

SAVEPOINT sp1;
来源：http://utk.fktsv.cn

ROLLBACK TO sp1;
来源：http://csp.yj202588.top

[Q69] 查看执行计划
来源：http://mdt.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uxh.yangfankeji.com

[Q70] 更新统计信息
来源：http://oiq.yuanzhike.top

ANALYZE TABLE users;
来源：http://pqm.shzxlz.cn

[Q71] 查看建表语句
来源：http://dhc.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rjd.fanxiaobao.xyz

[Q72] 查看索引
来源：http://odw.smart0.xyz

SHOW INDEX FROM users;
来源：http://mvs.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://hkp.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yrh.cdnleiting.top

[Q74] 强制使用索引
来源：http://ezc.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mvv.gzhubu.top

[Q75] 日期格式化
来源：http://ccv.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cvv.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pfw.nanxuanxn.top

[Q76] 按天统计
来源：http://kla.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jaq.tianlin.xyz

[Q77] 时间加减
来源：http://upo.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lgr.ppjwa.cn

[Q78] 当前时间
来源：http://spl.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nns.wangdashe.top

[Q79] 字符串拼接
来源：http://ngr.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fyj.xylfe.cn

[Q80] 字符串截取
来源：http://lhj.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cus.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://uys.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bfc.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://ffw.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qyy.yangfankeji.com

[Q83] 大小写转换
来源：http://hbs.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zny.cdnleiting.top

[Q84] 去除首尾空格
来源：http://zdd.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://axh.birdmap.top

[Q85] 数值取整
来源：http://diy.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uei.cheryme.top

[Q86] 读取 JSON 字段
来源：http://iun.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mdf.vehdjk.com

[Q87] JSON 字段做条件
来源：http://uvx.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uec.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://rqg.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qkb.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jfq.9152youxi.cn

[Q89] 判断表是否存在
来源：http://yjg.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hpm.cashguo.top

[Q90] 生成序号列
来源：http://fqv.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uca.xziqi.cn

================================================================================
来源：http://alv.jyoumei.cn

R. Bash 专题
来源：http://zpb.shuidangran.top

================================================================================
来源：http://acc.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://omu.jiagoushi.top

#!/usr/bin/env bash
来源：http://ayc.andypj.xyz

set -euo pipefail
来源：http://wtu.havefunace.top

[R02] 变量赋值与使用
来源：http://fhb.yueranfly.top

name="Tom"; echo "$name"
来源：http://cfp.jinqigufen.top

[R03] 只读变量
来源：http://gkv.gogol.net.cn

readonly PI=3.14
来源：http://esv.shzxlz.cn

[R04] 位置参数
来源：http://ppq.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hzx.shuidangran.top

[R05] 参数默认值
来源：http://wso.yj20258888.top

name="${1:-default}"
来源：http://imk.bbcook.cn

[R06] 判断命令是否存在
来源：http://wab.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wlb.zhoulong.xyz

[R07] if 判断文件
来源：http://zuz.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xon.feifeiyinyue.top

[R08] 数值比较
来源：http://wxr.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://epc.yanxiufei.cn

[R09] 字符串比较
来源：http://ulz.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sip.ydzc1.top

[R10] 正则匹配
来源：http://nmy.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ojs.shzxlz.cn

[R11] case 多分支
来源：http://dfd.yonumen.top

case "$1" in
来源：http://qio.ppjwa.cn

start) echo "启动" ;;
来源：http://gtn.xziqi.cn

stop)  echo "停止" ;;
来源：http://cvp.yj20258888.top

*)     echo "未知命令" ;;
来源：http://wlk.dianchejie.cn

esac
来源：http://vgn.dashuyun.cn

[R12] for 遍历文件
来源：http://fcq.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://iyp.quarkkingdee.top

[R13] for 计数循环
来源：http://gzd.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ysd.yfazqb.com

[R14] C 风格 for
来源：http://dmc.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qzk.jyoumei.cn

[R15] while 逐行读文件
来源：http://rys.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rro.yuanzhike.top

[R16] until 等待条件
来源：http://hkm.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://klj.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://ypp.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://mmv.epnwcf.com

[R18] 遍历数组
来源：http://bjg.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilv.nanxinkj.top

[R19] 数组长度
来源：http://rsp.vqdsnc.cn

echo "${#arr[@]}"
来源：http://nki.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://sbe.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vvl.fengsongda.top

[R21] 字符串长度
来源：http://sjw.xziqi.cn

echo "${#s}"
来源：http://ihx.ywan-chungtsiang.top

[R22] 截取子串
来源：http://njm.xinyue.icu

echo "${s:0:5}"
来源：http://mov.yongpay.top

[R23] 字符串替换
来源：http://iuf.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://akl.sxryk.cn

[R24] 大小写转换
来源：http://okf.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uvq.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://ibt.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zqq.yj20258.top

[R26] 命令替换
来源：http://xgd.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://lvy.jinghuilouyu.cn

[R27] 算术展开
来源：http://eye.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://fbk.birdmap.top

[R28] 浮点运算
来源：http://ozl.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://jko.bjfxy.top

[R29] 定义函数
来源：http://zmp.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://szm.zhixingplan.top

[R30] 函数返回状态码
来源：http://huk.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://dhe.zdqjudy.top

[R31] 局部变量
来源：http://otg.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://zay.hesvh.cn

[R32] 参数个数校验
来源：http://zgn.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyl.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://xex.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://avg.mhx1999.top

[R34] 退出时清理
来源：http://ydm.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fcf.bjfxy.top

[R35] 后台执行并等待
来源：http://zor.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kzh.yueranfly.top

[R36] 并发执行多个任务
来源：http://iuj.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cah.meibo888.top

[R37] 把输出赋给变量
来源：http://tdv.tarul.cn

files=$(ls -1)
来源：http://vud.hongshengwenyu.top

[R38] 管道串联
来源：http://nnx.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://krh.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://dkz.fehbvm.com

cmd > out.log 2>&1
来源：http://tbe.smart0.xyz

[R40] 追加写日志
来源：http://num.fzhhl.top

echo "log" >> out.log
来源：http://ide.zhongyouzk.top

[R41] 丢弃输出
来源：http://cxb.xuanzx.com

cmd >/dev/null 2>&1
来源：http://myd.haohaochexian.top

[R42] 输入重定向
来源：http://ven.birdmap.top

wc -l < a.txt
来源：http://kgj.hesvh.cn

[R43] 按名字查找文件
来源：http://fhi.sufxvd.cn

find . -name "*.log" -type f
来源：http://com.fengsongda.top

[R44] 按修改时间查找
来源：http://ojx.0kj1m.cn

find . -mtime -7 -type f
来源：http://zqv.zycfv.cn

[R45] 批量删除
来源：http://pun.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://jiw.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://ajd.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zqn.uphjek.com

[R47] sed 单行替换
来源：http://ees.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cum.0kj1m.cn

[R48] awk 取指定列
来源：http://djb.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://qtu.ppjwa.cn

[R49] awk 带条件
来源：http://ngk.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pti.c1oappe.top

[R50] awk 求和
来源：http://hev.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://gwa.vqdsnc.cn

[R51] 排序去重取前几
来源：http://ifj.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dhe.nanxinkj.top

[R52] 统计行数
来源：http://ugj.cashguo.top

wc -l a.txt
来源：http://utq.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://ebj.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zrv.ctjpmb.com

[R54] 比较两个文件
来源：http://xxw.iojbl.cn

diff a.txt b.txt
来源：http://htj.jyoumei.cn

[R55] 压缩与解压
来源：http://bdv.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mvi.sysykeji.top

[R56] 远程拷贝
来源：http://ylw.aibaodan.cn

scp file user@host:/path/
来源：http://yyi.zhoulong.xyz

[R57] 远程执行命令
来源：http://wou.jlsjyb.cn

ssh user@host 'uptime'
来源：http://ela.gotoacloud.top

[R58] 下载文件
来源：http://ogy.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bdz.aibaodan.cn

[R59] 发 POST JSON
来源：http://ort.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sxm.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://yoz.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xcp.xuetiantiany.cn

[R61] 磁盘占用
来源：http://lnp.chenzaomai.com

df -h;  du -sh *
来源：http://ngv.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://xas.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://zyf.yuanzhike.top

[R63] 内存与进程
来源：http://pkw.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://akh.aizwys.cn

[R64] 结束进程
来源：http://wcb.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://opu.cqqwz.cn

[R65] 查看端口占用
来源：http://vvg.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xdh.andypj.xyz

[R66] 定时任务
来源：http://cgi.jqgfzy.top

crontab -e;  crontab -l
来源：http://mgz.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://lbo.xinyue.icu

openssl rand -hex 16
来源：http://exz.cqqwz.cn

[R68] 计算文件校验值
来源：http://ysr.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ybq.jlsjyb.cn

[R69] 生成随机密码
来源：http://ifj.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://qpz.ehwqpu.com

[R70] 时间戳与互转
来源：http://lmu.hnqzz.top

date +%s;  date -d @1700000000
来源：http://tws.9152youxi.cn

[R71] 日期格式化
来源：http://sob.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eku.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://mux.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gvf.hnxiangtu.top

[R73] 分割大日志
来源：http://rxg.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://oey.guowangkeji.top

[R74] 批量重命名
来源：http://dsr.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xwz.tianlin.xyz

[R75] 导出环境变量
来源：http://daq.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://fiu.kuanghao11.cn

[R76] 使用临时文件
来源：http://hwd.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zea.zhixingplan.top

[R77] 读取用户输入
来源：http://bfh.bjfxy.top

read -rp "请输入: " ans
来源：http://cxh.cashguo.top

[R78] 交互式菜单
来源：http://gak.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wtw.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://daf.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mpa.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://psg.redwolf501.top

time ./run.sh
来源：http://qfd.fktsv.cn

================================================================================
来源：http://idt.chenlongwang.top

S. C / C++ 专题
来源：http://fwb.meibo888.top

================================================================================
来源：http://gmg.yonumen.top

[S01] C：Hello World
来源：http://gjw.yueranfly.top

#include <stdio.h>
来源：http://lny.dianchejie.cn


<!-- 参考信息 -->