代发 wailian999

[Q33] 多列分组
来源：http://lgp.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uup.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://ypy.cheryme.top

SELECT * FROM (
来源：http://xry.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ema.wangdashe.top

) t WHERE rn = 1;
来源：http://wya.fzhhl.top

[Q35] 内连接
来源：http://coo.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sjh.yuxming.cn

[Q36] 左连接
来源：http://yca.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rii.fktsv.cn

[Q37] 右连接
来源：http://bxp.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mmu.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://ixg.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wgg.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://qzh.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqt.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://erh.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lrn.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lwa.zhoulong.xyz

[Q41] 多表连接
来源：http://gtt.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nxb.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://vsj.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://gaj.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://kou.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://adl.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dgf.xziqi.cn

[Q43] 标量子查询
来源：http://gvo.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://huq.chenlongwang.top

[Q44] IN 子查询
来源：http://orq.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dew.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://onf.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fnc.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cob.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yml.wangdashe.top

[Q47] 与平均值比较
来源：http://bvg.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ibq.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://dxc.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xkp.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://uye.birdmap.top

[Q49] 更新单行
来源：http://snn.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://glo.gotoacloud.top

[Q50] 批量更新
来源：http://fey.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nwr.zhijiandao.cn

[Q51] 用子查询更新
来源：http://iuw.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxq.yuanzhike.top

[Q52] 删除指定行
来源：http://suf.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://hnx.hywenlv.cn

[Q53] 按条件删除
来源：http://ndm.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sfc.gaohongyu789.top

[Q54] 清空表
来源：http://ant.xuanzx.com

TRUNCATE TABLE logs;
来源：http://ous.yj20258888.top

[Q55] 排名（并列占位）
来源：http://zmm.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://egm.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://bwg.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jnc.daria6918.cn

[Q57] 行号
来源：http://leg.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bdk.xylfe.cn

[Q58] 累计求和
来源：http://dvd.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nih.yvedp.cn

[Q59] 分组内累计
来源：http://ryv.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ibh.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://hnn.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oye.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uov.sweek.top

[Q61] 移动平均
来源：http://vbw.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zvp.xylfe.cn

[Q62] 分组占比
来源：http://vkw.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://epq.daria6918.cn

[Q63] 开启事务
来源：http://gbr.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://yxz.cashguo.top

[Q64] 提交事务
来源：http://ayi.zhongyouzk.top

COMMIT;
来源：http://icl.tarul.cn

[Q65] 回滚事务
来源：http://zbw.zdqjudy.top

ROLLBACK;
来源：http://ias.ybcxt.top

[Q66] 行锁查询
来源：http://nfv.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://huk.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://ikd.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vyz.c1oappe.top

[Q68] 保存点
来源：http://ezg.zhongyouzk.top

SAVEPOINT sp1;
来源：http://qtq.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://foa.sxryk.cn

[Q69] 查看执行计划
来源：http://fjj.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fvw.daria6918.cn

[Q70] 更新统计信息
来源：http://hub.cucudq.cn

ANALYZE TABLE users;
来源：http://sgt.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://frn.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cnv.52xcode.cn

[Q72] 查看索引
来源：http://kbh.gzhubu.top

SHOW INDEX FROM users;
来源：http://jmr.nwbrower.top

[Q73] 查看表状态
来源：http://kmp.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rzf.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://fza.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xru.redwolf501.top

[Q75] 日期格式化
来源：http://nox.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gwd.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zdj.zdbjq.cn

[Q76] 按天统计
来源：http://gkk.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://njb.yongpay.top

[Q77] 时间加减
来源：http://ikd.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vuz.hnqzz.top

[Q78] 当前时间
来源：http://xpp.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jrr.quarkkingdee.top

[Q79] 字符串拼接
来源：http://ooz.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://csh.jqgfzy.top

[Q80] 字符串截取
来源：http://tyl.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lpn.zycfv.cn

[Q81] 字符串替换
来源：http://gvx.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hhr.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://dup.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jot.jinqigfzy.top

[Q83] 大小写转换
来源：http://srj.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xjp.c1oappe.top

[Q84] 去除首尾空格
来源：http://npr.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://ozq.smart0.xyz

[Q85] 数值取整
来源：http://igt.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://syi.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://pyh.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://keh.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://jah.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gks.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://vuw.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aiv.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://idb.yongpay.top

[Q89] 判断表是否存在
来源：http://biy.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iuy.svipenyu.cn

[Q90] 生成序号列
来源：http://ctp.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mzg.zycfv.cn

================================================================================
来源：http://inp.ppjwa.cn

R. Bash 专题
来源：http://her.hfpthk.cn

================================================================================
来源：http://gwg.fehbvm.com

[R01] shebang 与严格模式
来源：http://alx.zycfv.cn

#!/usr/bin/env bash
来源：http://lzs.tian-w.cn

set -euo pipefail
来源：http://jzl.hfpthk.cn

[R02] 变量赋值与使用
来源：http://rnr.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://jms.zhongyouzk.top

[R03] 只读变量
来源：http://stp.gaohongyu789.top

readonly PI=3.14
来源：http://rwa.cqqwz.cn

[R04] 位置参数
来源：http://pjz.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvb.sysykeji.top

[R05] 参数默认值
来源：http://oko.fengsongda.top

name="${1:-default}"
来源：http://hax.hysaishi.cn

[R06] 判断命令是否存在
来源：http://ady.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pbh.hcnkem.com

[R07] if 判断文件
来源：http://mua.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jka.0kj1m.cn

[R08] 数值比较
来源：http://nmv.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://lia.dashuyun.cn

[R09] 字符串比较
来源：http://bxd.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://juw.hongshengwenyu.top

[R10] 正则匹配
来源：http://foy.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jvw.cqqwz.cn

[R11] case 多分支
来源：http://wnt.tarul.cn

case "$1" in
来源：http://wgu.316326.xyz

start) echo "启动" ;;
来源：http://buy.ctjpmb.com

stop)  echo "停止" ;;
来源：http://mos.yj202588.top

*)     echo "未知命令" ;;
来源：http://mfq.daxiang520.top

esac
来源：http://lgu.hcnkem.com

[R12] for 遍历文件
来源：http://lnl.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://ynh.jiagoushi.top

[R13] for 计数循环
来源：http://dua.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://szh.daria6918.cn

[R14] C 风格 for
来源：http://fpx.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://euo.quarkkingdee.top

[R15] while 逐行读文件
来源：http://kei.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mcs.xziqi.cn

[R16] until 等待条件
来源：http://jjm.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jkc.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://lox.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://mnl.sufxvd.cn

[R18] 遍历数组
来源：http://uqj.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ark.tanke756.top

[R19] 数组长度
来源：http://vgh.tanke756.top

echo "${#arr[@]}"
来源：http://vco.tarul.cn

[R20] 关联数组（字典）
来源：http://ejw.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ntk.shangyingyoupin.top

[R21] 字符串长度
来源：http://kix.vehdjk.com

echo "${#s}"
来源：http://wuy.xuanzx.com

[R22] 截取子串
来源：http://ahr.fehbvm.com

echo "${s:0:5}"
来源：http://tjm.bjfxy.top

[R23] 字符串替换
来源：http://qfj.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qsl.yongpay.top

[R24] 大小写转换
来源：http://ykd.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jrq.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://xwc.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xte.zdqjudy.top

[R26] 命令替换
来源：http://fvq.yonumen.top

now=$(date +%F); echo "$now"
来源：http://mra.birdmap.top

[R27] 算术展开
来源：http://goz.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://pkq.chenlongwang.top

[R28] 浮点运算
来源：http://iuw.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://bpp.jqgfzy.top

[R29] 定义函数
来源：http://xsg.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxj.cashguo.top

[R30] 函数返回状态码
来源：http://bpn.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://fqc.zhaomingkeji.xyz

[R31] 局部变量
来源：http://pgx.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://acn.nanxuanxn.top

[R32] 参数个数校验
来源：http://umg.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ymn.yj202588.top

[R33] 捕获错误并提示行号
来源：http://gvp.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://etw.yongpay.top

[R34] 退出时清理
来源：http://nln.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gfe.chenlongwang.top

[R35] 后台执行并等待
来源：http://hiw.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://syd.gogol.net.cn

[R36] 并发执行多个任务
来源：http://pia.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ivv.chenlongwang.top

[R37] 把输出赋给变量
来源：http://ewa.c1oappe.top

files=$(ls -1)
来源：http://qmq.quarkkingdee.top

[R38] 管道串联
来源：http://szd.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://uyx.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://xuv.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://qde.zhijiandao.cn

[R40] 追加写日志
来源：http://icp.gogol.net.cn

echo "log" >> out.log
来源：http://gbp.redwolf501.top

[R41] 丢弃输出
来源：http://dew.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://jxl.zhoulong.xyz

[R42] 输入重定向
来源：http://cst.daria6918.cn

wc -l < a.txt
来源：http://eok.hfpthk.cn

[R43] 按名字查找文件
来源：http://kjw.xinyue.icu

find . -name "*.log" -type f
来源：http://uox.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://vla.haohaochexian.top

find . -mtime -7 -type f
来源：http://yji.cdnleiting.top

[R45] 批量删除
来源：http://jzy.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://zfo.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://rlt.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mtw.shangyingyoupin.top

[R47] sed 单行替换
来源：http://qui.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cmk.vqdsnc.cn

[R48] awk 取指定列
来源：http://pbi.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://cho.guannengcc.top

[R49] awk 带条件
来源：http://sic.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://srx.316326.xyz

[R50] awk 求和
来源：http://bia.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://pmh.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://swe.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iuk.zycfv.cn

[R52] 统计行数
来源：http://wwf.316326.xyz

wc -l a.txt
来源：http://kcn.sweek.top

[R53] 查看文件头与实时尾
来源：http://rjp.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uht.zdbjq.cn

[R54] 比较两个文件
来源：http://kdr.cdnleiting.top

diff a.txt b.txt
来源：http://mcb.haohaochexian.top

[R55] 压缩与解压
来源：http://chz.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykj.fehbvm.com

[R56] 远程拷贝
来源：http://awk.zdbjq.cn

scp file user@host:/path/
来源：http://wgf.xuetiantiany.cn

[R57] 远程执行命令
来源：http://qvb.fktsv.cn

ssh user@host 'uptime'
来源：http://utx.sweek.top

[R58] 下载文件
来源：http://xhl.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wjr.nanxinkj.top

[R59] 发 POST JSON
来源：http://tpz.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kdy.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://wiy.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mmd.hesvh.cn

[R61] 磁盘占用
来源：http://wta.zhixingplan.top

df -h;  du -sh *
来源：http://ada.haohaochexian.top

[R62] 找最占空间的文件
来源：http://fxu.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://tec.tanke756.top

[R63] 内存与进程
来源：http://kop.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://uth.chenzaomai.com

[R64] 结束进程
来源：http://tao.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://klj.zhiwuduotai.top

[R65] 查看端口占用
来源：http://qig.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rhl.mhx1999.top

[R66] 定时任务
来源：http://aif.vqdsnc.cn

crontab -e;  crontab -l
来源：http://hws.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://esw.daria6918.cn

openssl rand -hex 16
来源：http://jkw.dashuyun.cn

[R68] 计算文件校验值
来源：http://nbv.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://kwv.sweek.top

[R69] 生成随机密码
来源：http://rek.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://weu.bjfxy.top

[R70] 时间戳与互转
来源：http://lai.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://adf.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://qzq.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rxo.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://aqu.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://kvp.xuetiantiany.cn

[R73] 分割大日志
来源：http://omu.sweek.top

split -l 1000 big.log part_
来源：http://xxh.zhengqikj.top

[R74] 批量重命名
来源：http://wlw.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cdz.jianghu66.top

[R75] 导出环境变量
来源：http://mke.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://smh.jqgufenzy.top

[R76] 使用临时文件
来源：http://tkd.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gqi.ppjwa.cn

[R77] 读取用户输入
来源：http://kos.cheryme.top

read -rp "请输入: " ans
来源：http://ywl.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://rfl.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vxv.mhx1999.top

[R79] 解析命令行选项
来源：http://wcs.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://acf.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://rpb.hnqzz.top

time ./run.sh
来源：http://syb.birdmap.top

================================================================================
来源：http://aik.snrcjt.cn

S. C / C++ 专题
来源：http://gvj.9152youxi.cn

================================================================================
来源：http://uom.quarkkingdee.top

[S01] C：Hello World
来源：http://nnd.xinyue.icu

#include <stdio.h>
来源：http://xxs.redwolf501.top


<!-- 参考信息 -->