代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kiz.sysykeji.top

[Q28] 求和与平均
来源：http://ona.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cmj.ppjwa.cn

[Q29] 最大最小值
来源：http://rgu.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://doe.hnxiangtu.top

[Q30] 分组统计
来源：http://lsf.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cza.hysaishi.cn

[Q31] 分组后过滤
来源：http://zwb.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pxg.yj20258.top

[Q32] 分组拼接字符串
来源：http://gpx.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lsx.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wav.yongpay.top

[Q33] 多列分组
来源：http://yrg.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gmy.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://gid.jyoumei.cn

SELECT * FROM (
来源：http://lzm.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cxp.guannengcc.top

) t WHERE rn = 1;
来源：http://mjo.yonumen.top

[Q35] 内连接
来源：http://mhl.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ean.tanke756.top

[Q36] 左连接
来源：http://daq.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pbd.nanxuanxn.top

[Q37] 右连接
来源：http://tal.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mhz.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gfv.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gli.ivvv.top

[Q39] 自连接（查上下级）
来源：http://jvz.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vau.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vqv.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gys.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://diz.yfazqb.com

[Q41] 多表连接
来源：http://bhc.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fmq.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://eac.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://bvu.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://xso.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://vbw.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://clh.hammf.cn

[Q43] 标量子查询
来源：http://rmg.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qoo.jqgufenzy.top

[Q44] IN 子查询
来源：http://yoh.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uhu.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://mip.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkw.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://zqt.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://svo.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://sfe.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aaf.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://stv.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ntp.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://pye.shangyingyoupin.top

[Q49] 更新单行
来源：http://tzs.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://upi.vqdsnc.cn

[Q50] 批量更新
来源：http://mlw.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wus.andypj.xyz

[Q51] 用子查询更新
来源：http://riw.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mgi.tanke756.top

[Q52] 删除指定行
来源：http://pyq.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://hxj.yj20258888.top

[Q53] 按条件删除
来源：http://ttj.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cqr.hysaishi.cn

[Q54] 清空表
来源：http://xph.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://qgd.c1oappe.top

[Q55] 排名（并列占位）
来源：http://svg.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fsb.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://wdu.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lhd.quarkkingdee.top

[Q57] 行号
来源：http://wbm.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xtj.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://bcm.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxz.gotoacloud.top

[Q59] 分组内累计
来源：http://jtw.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xyb.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://cex.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmw.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://syo.shanyushiyangtech.top

[Q61] 移动平均
来源：http://qfa.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ofs.tian-w.cn

[Q62] 分组占比
来源：http://nbv.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aah.jlsjyb.cn

[Q63] 开启事务
来源：http://jmf.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ckl.snrcjt.cn

[Q64] 提交事务
来源：http://dnm.yj202588.top

COMMIT;
来源：http://rzn.daxiang520.top

[Q65] 回滚事务
来源：http://pkj.uphjek.com

ROLLBACK;
来源：http://pcv.zycfv.cn

[Q66] 行锁查询
来源：http://ona.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vnz.jinqigufen.top

[Q67] 设置隔离级别
来源：http://znh.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jkd.0kj1m.cn

[Q68] 保存点
来源：http://ykd.zhoulong.xyz

SAVEPOINT sp1;
来源：http://jit.bbcook.cn

ROLLBACK TO sp1;
来源：http://kny.cucudq.cn

[Q69] 查看执行计划
来源：http://sfv.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zsz.ydjk.org.cn

[Q70] 更新统计信息
来源：http://iqa.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://ptt.fengsongda.top

[Q71] 查看建表语句
来源：http://uiv.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lzr.zhongyouzk.top

[Q72] 查看索引
来源：http://jmm.52xcode.cn

SHOW INDEX FROM users;
来源：http://gcc.wangdashe.top

[Q73] 查看表状态
来源：http://irn.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://gge.zhongyouzk.top

[Q74] 强制使用索引
来源：http://jzp.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sps.quarkkingdee.top

[Q75] 日期格式化
来源：http://chk.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dzt.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uko.yueranfly.top

[Q76] 按天统计
来源：http://wft.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gih.havefunace.top

[Q77] 时间加减
来源：http://fve.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://orv.xuanzx.com

[Q78] 当前时间
来源：http://gak.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sly.quarkkingdee.top

[Q79] 字符串拼接
来源：http://eaq.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nev.ydzc1.top

[Q80] 字符串截取
来源：http://uyp.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://got.zhengqikj.top

[Q81] 字符串替换
来源：http://jwz.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dvv.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://wxs.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uqi.kuanghao11.cn

[Q83] 大小写转换
来源：http://wyx.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbx.yangfankeji.com

[Q84] 去除首尾空格
来源：http://uhy.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://bwr.sjlbkw.cn

[Q85] 数值取整
来源：http://hxm.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ojf.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://scc.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jgg.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://dst.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dpm.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://kkf.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fca.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lag.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://gzq.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lax.yj20258888.top

[Q90] 生成序号列
来源：http://buf.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xby.52xcode.cn

================================================================================
来源：http://agk.9152youxi.cn

R. Bash 专题
来源：http://ezg.cheryme.top

================================================================================
来源：http://kjr.gzhubu.top

[R01] shebang 与严格模式
来源：http://nty.ehwqpu.com

#!/usr/bin/env bash
来源：http://hzu.yuxming.cn

set -euo pipefail
来源：http://bep.snrcjt.cn

[R02] 变量赋值与使用
来源：http://vfz.ybcxt.top

name="Tom"; echo "$name"
来源：http://kio.yj202588.top

[R03] 只读变量
来源：http://ipw.sufxvd.cn

readonly PI=3.14
来源：http://vzu.wangshuangyany.cn

[R04] 位置参数
来源：http://zdn.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mnw.aizwys.cn

[R05] 参数默认值
来源：http://ech.hnxiangtu.top

name="${1:-default}"
来源：http://mss.cqqwz.cn

[R06] 判断命令是否存在
来源：http://xqb.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kqf.shuidangran.top

[R07] if 判断文件
来源：http://qsi.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vvc.jiagoushi.top

[R08] 数值比较
来源：http://hlu.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://scl.cqqwz.cn

[R09] 字符串比较
来源：http://uzs.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://puu.chenlongwang.top

[R10] 正则匹配
来源：http://jqr.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://noe.cdnleiting.top

[R11] case 多分支
来源：http://ned.tianlin.xyz

case "$1" in
来源：http://mal.c1oappe.top

start) echo "启动" ;;
来源：http://yuk.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://aho.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://dak.gogol.net.cn

esac
来源：http://jex.cdnleiting.top

[R12] for 遍历文件
来源：http://pnm.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://xgj.jlsjyb.cn

[R13] for 计数循环
来源：http://did.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://pky.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://jeg.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kai.ppjwa.cn

[R15] while 逐行读文件
来源：http://brh.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jzz.ydjk.org.cn

[R16] until 等待条件
来源：http://aah.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lzp.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://sxd.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://toy.andypj.xyz

[R18] 遍历数组
来源：http://wzq.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ixq.wangdashe.top

[R19] 数组长度
来源：http://brf.xinyue.icu

echo "${#arr[@]}"
来源：http://nkg.gogol.net.cn

[R20] 关联数组（字典）
来源：http://ryj.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vop.yvedp.cn

[R21] 字符串长度
来源：http://jyu.vehdjk.com

echo "${#s}"
来源：http://nns.guowangkeji.top

[R22] 截取子串
来源：http://hrh.xinyue.icu

echo "${s:0:5}"
来源：http://ocb.cheryme.top

[R23] 字符串替换
来源：http://rjk.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pet.yanxiufei.cn

[R24] 大小写转换
来源：http://wac.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://ush.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://njb.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ryn.hammf.cn

[R26] 命令替换
来源：http://zpw.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://yre.shuidangran.top

[R27] 算术展开
来源：http://bfa.yfazqb.com

echo $((1 + 2 * 3))
来源：http://usv.xinyue.icu

[R28] 浮点运算
来源：http://lnk.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://ihl.dashuyun.cn

[R29] 定义函数
来源：http://lvu.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfe.nanxinkj.top

[R30] 函数返回状态码
来源：http://ocp.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://izl.jyoumei.cn

[R31] 局部变量
来源：http://ylp.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://plf.wangdashe.top

[R32] 参数个数校验
来源：http://buw.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dbx.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://tcy.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://own.316326.xyz

[R34] 退出时清理
来源：http://xmr.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mdd.zhoulong.xyz

[R35] 后台执行并等待
来源：http://vqk.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xbc.snrcjt.cn

[R36] 并发执行多个任务
来源：http://uwx.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qfi.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://wbg.fanxiaobao.xyz

files=$(ls -1)
来源：http://qls.ydjk.org.cn

[R38] 管道串联
来源：http://isz.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://rbv.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://ols.andypj.xyz

cmd > out.log 2>&1
来源：http://nap.zhongyouzk.top

[R40] 追加写日志
来源：http://kof.haohaochexian.top

echo "log" >> out.log
来源：http://bcq.xuetiantiany.cn

[R41] 丢弃输出
来源：http://dik.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://ebi.ppjwa.cn

[R42] 输入重定向
来源：http://qoq.jinqigufen.top

wc -l < a.txt
来源：http://xut.hnqzz.top

[R43] 按名字查找文件
来源：http://etz.cucudq.cn

find . -name "*.log" -type f
来源：http://yqq.mhx1999.top

[R44] 按修改时间查找
来源：http://edu.bjfxy.top

find . -mtime -7 -type f
来源：http://vpn.shzxlz.cn

[R45] 批量删除
来源：http://imq.yonumen.top

find . -name "*.tmp" -delete
来源：http://tsy.nanxinkj.top

[R46] 递归替换文件内容
来源：http://tvz.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bys.bjfxy.top

[R47] sed 单行替换
来源：http://wkj.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://tdz.shuidangran.top

[R48] awk 取指定列
来源：http://utv.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://asf.hnqzz.top

[R49] awk 带条件
来源：http://zih.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ctl.fktsv.cn

[R50] awk 求和
来源：http://bun.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ngd.ydzc1.top

[R51] 排序去重取前几
来源：http://jss.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xia.yonumen.top

[R52] 统计行数
来源：http://buj.zhaomingkeji.xyz

wc -l a.txt
来源：http://pxs.yj202588.top

[R53] 查看文件头与实时尾
来源：http://vli.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pvt.xziqi.cn

[R54] 比较两个文件
来源：http://vwq.pycfn.com

diff a.txt b.txt
来源：http://vkr.nanxuanxn.top

[R55] 压缩与解压
来源：http://sqz.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jmu.jiagoushi.top

[R56] 远程拷贝
来源：http://ztm.xuetiantiany.cn

scp file user@host:/path/
来源：http://rjf.yj20258888.top

[R57] 远程执行命令
来源：http://zaz.316326.xyz

ssh user@host 'uptime'
来源：http://ywl.aibaodan.cn

[R58] 下载文件
来源：http://ysg.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jjv.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://kiu.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ien.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://lee.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yay.gaohongyu789.top

[R61] 磁盘占用
来源：http://crv.zycfv.cn

df -h;  du -sh *
来源：http://iqd.zdqjudy.top

[R62] 找最占空间的文件
来源：http://fjw.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://vfs.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://quc.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://rzl.ehwqpu.com

[R64] 结束进程
来源：http://cyf.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://fvz.jqgufenzy.top

[R65] 查看端口占用
来源：http://zgl.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hzp.sufxvd.cn

[R66] 定时任务
来源：http://yju.ydjk.org.cn

crontab -e;  crontab -l
来源：http://nlh.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://xme.pycfn.com

openssl rand -hex 16
来源：http://wtw.mhx1999.top

[R68] 计算文件校验值
来源：http://ooi.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vjr.yj202588.top

[R69] 生成随机密码
来源：http://lar.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://fnb.yj20258888.top

[R70] 时间戳与互转
来源：http://oky.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://rxe.cqqwz.cn

[R71] 日期格式化
来源：http://lwl.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pgq.jqgufenzy.top

[R72] 等待端口就绪
来源：http://gfh.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://abk.iojbl.cn

[R73] 分割大日志
来源：http://mbc.andypj.xyz

split -l 1000 big.log part_
来源：http://kvv.xuanzx.com

[R74] 批量重命名
来源：http://umf.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mlk.ydzc1.top

[R75] 导出环境变量
来源：http://tic.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://ved.ybcxt.top

[R76] 使用临时文件
来源：http://otw.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lge.ybcxt.top

[R77] 读取用户输入
来源：http://jhn.c1oappe.top


<!-- 参考信息 -->