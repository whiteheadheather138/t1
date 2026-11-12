代发 wailian999

[Q36] 左连接
来源：http://rwe.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oyu.epnwcf.com

[Q37] 右连接
来源：http://wwr.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvl.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tug.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qef.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://hcb.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ykh.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zck.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vzf.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tas.ydjk.org.cn

[Q41] 多表连接
来源：http://ixx.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wun.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://bbd.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://vat.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://jri.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://ujv.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://weh.ctjpmb.com

[Q43] 标量子查询
来源：http://xmm.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eka.zhoulong.xyz

[Q44] IN 子查询
来源：http://psl.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xwb.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://cua.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsa.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mjl.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ueh.aibaodan.cn

[Q47] 与平均值比较
来源：http://dio.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://orw.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://lmv.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yjq.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://oye.jiagoushi.top

[Q49] 更新单行
来源：http://nhx.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yts.svipenyu.cn

[Q50] 批量更新
来源：http://zua.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://svx.bbcook.cn

[Q51] 用子查询更新
来源：http://tpv.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npo.epnwcf.com

[Q52] 删除指定行
来源：http://erb.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://jnh.9152youxi.cn

[Q53] 按条件删除
来源：http://vwd.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pgx.aizwys.cn

[Q54] 清空表
来源：http://ort.sysykeji.top

TRUNCATE TABLE logs;
来源：http://aww.yongpay.top

[Q55] 排名（并列占位）
来源：http://tmt.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://djg.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://epu.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dua.yj202588.top

[Q57] 行号
来源：http://jbb.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xnp.yj20258888.top

[Q58] 累计求和
来源：http://pim.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kag.shuidangran.top

[Q59] 分组内累计
来源：http://wwd.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mct.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://gzw.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aup.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wok.zhengqikj.top

[Q61] 移动平均
来源：http://upu.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bib.sysykeji.top

[Q62] 分组占比
来源：http://kza.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://buj.quarkkingdee.top

[Q63] 开启事务
来源：http://jxp.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qpe.yangfankeji.com

[Q64] 提交事务
来源：http://tpo.xingfuxueyuan.xyz

COMMIT;
来源：http://xng.sysykeji.top

[Q65] 回滚事务
来源：http://jsv.tarul.cn

ROLLBACK;
来源：http://xra.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://lra.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bbw.cashguo.top

[Q67] 设置隔离级别
来源：http://iit.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xco.cashguo.top

[Q68] 保存点
来源：http://ixa.sxryk.cn

SAVEPOINT sp1;
来源：http://emt.jyoumei.cn

ROLLBACK TO sp1;
来源：http://rwa.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://exw.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gbk.tarul.cn

[Q70] 更新统计信息
来源：http://sgd.gogol.net.cn

ANALYZE TABLE users;
来源：http://exu.52xcode.cn

[Q71] 查看建表语句
来源：http://xaw.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pcl.316326.xyz

[Q72] 查看索引
来源：http://fva.epnwcf.com

SHOW INDEX FROM users;
来源：http://vva.vqdsnc.cn

[Q73] 查看表状态
来源：http://dsj.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://icj.yueranfly.top

[Q74] 强制使用索引
来源：http://fgs.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kxc.iojbl.cn

[Q75] 日期格式化
来源：http://rlg.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cvz.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rhk.svipenyu.cn

[Q76] 按天统计
来源：http://svy.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vqd.jyoumei.cn

[Q77] 时间加减
来源：http://zbl.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bai.quarkkingdee.top

[Q78] 当前时间
来源：http://dem.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dpi.yfazqb.com

[Q79] 字符串拼接
来源：http://ikj.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bkn.fengsongda.top

[Q80] 字符串截取
来源：http://cyt.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hcw.gzhubu.top

[Q81] 字符串替换
来源：http://jez.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hqm.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://dvc.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nzz.zhengqikj.top

[Q83] 大小写转换
来源：http://xva.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xnm.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://hkr.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://nzm.havefunace.top

[Q85] 数值取整
来源：http://pdh.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aoh.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://fwg.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tme.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://zod.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://glo.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://uhm.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eqh.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eej.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://lrq.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wwj.chenlongwang.top

[Q90] 生成序号列
来源：http://vha.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iod.zdbjq.cn

================================================================================
来源：http://chu.chenzaomai.com

R. Bash 专题
来源：http://dog.zhiwuduotai.top

================================================================================
来源：http://ipc.hcnkem.com

[R01] shebang 与严格模式
来源：http://ofe.yuanzhike.top

#!/usr/bin/env bash
来源：http://xsi.nanxuanxn.top

set -euo pipefail
来源：http://wor.chenzaomai.com

[R02] 变量赋值与使用
来源：http://vog.fengsongda.top

name="Tom"; echo "$name"
来源：http://jsw.redwolf501.top

[R03] 只读变量
来源：http://dcn.yueranfly.top

readonly PI=3.14
来源：http://adw.gzhubu.top

[R04] 位置参数
来源：http://ayz.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://scl.yvedp.cn

[R05] 参数默认值
来源：http://fah.cheryme.top

name="${1:-default}"
来源：http://ulg.shuidangran.top

[R06] 判断命令是否存在
来源：http://xsz.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tjs.dashuyun.cn

[R07] if 判断文件
来源：http://jmd.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ywn.yuxming.cn

[R08] 数值比较
来源：http://wcw.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nqh.jiagoushi.top

[R09] 字符串比较
来源：http://hsg.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hxz.snrcjt.cn

[R10] 正则匹配
来源：http://suj.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qsg.epnwcf.com

[R11] case 多分支
来源：http://qjm.xziqi.cn

case "$1" in
来源：http://lcx.guowangkeji.top

start) echo "启动" ;;
来源：http://fxr.fktsv.cn

stop)  echo "停止" ;;
来源：http://ojk.jianghu66.top

*)     echo "未知命令" ;;
来源：http://kxv.hywenlv.cn

esac
来源：http://vhj.yj20258888.top

[R12] for 遍历文件
来源：http://qoi.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://nsm.kuanghao11.cn

[R13] for 计数循环
来源：http://xrj.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://hlg.fanxiaobao.xyz

[R14] C 风格 for
来源：http://lxr.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yha.xinyue.icu

[R15] while 逐行读文件
来源：http://gmv.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://utf.yj202588.top

[R16] until 等待条件
来源：http://dwu.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jyc.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://nsu.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://cuq.svipenyu.cn

[R18] 遍历数组
来源：http://blu.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vhx.xylfe.cn

[R19] 数组长度
来源：http://mkc.ctjpmb.com

echo "${#arr[@]}"
来源：http://bwv.cheryme.top

[R20] 关联数组（字典）
来源：http://skr.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ieb.ehwqpu.com

[R21] 字符串长度
来源：http://awb.cdnleiting.top

echo "${#s}"
来源：http://goe.fzhhl.top

[R22] 截取子串
来源：http://hzs.ctjpmb.com

echo "${s:0:5}"
来源：http://cud.yongpay.top

[R23] 字符串替换
来源：http://hej.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://igb.yueranfly.top

[R24] 大小写转换
来源：http://bgv.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gbf.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://nok.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbw.9152youxi.cn

[R26] 命令替换
来源：http://aod.cheryme.top

now=$(date +%F); echo "$now"
来源：http://scc.jlsjyb.cn

[R27] 算术展开
来源：http://bes.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://lkf.guannengcc.top

[R28] 浮点运算
来源：http://guf.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://jnb.cqqwz.cn

[R29] 定义函数
来源：http://jhl.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eck.tarul.cn

[R30] 函数返回状态码
来源：http://uea.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://pkq.jinghuilouyu.cn

[R31] 局部变量
来源：http://nxl.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://kfe.daxiang520.top

[R32] 参数个数校验
来源：http://ers.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dvh.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://glt.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ilt.bbcook.cn

[R34] 退出时清理
来源：http://vhs.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ivf.fehbvm.com

[R35] 后台执行并等待
来源：http://cab.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://aeb.tarul.cn

[R36] 并发执行多个任务
来源：http://dho.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ahs.fzhhl.top

[R37] 把输出赋给变量
来源：http://rqj.ehwqpu.com

files=$(ls -1)
来源：http://knp.zhongyouzk.top

[R38] 管道串联
来源：http://bql.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://piy.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://guo.cdnleiting.top

cmd > out.log 2>&1
来源：http://dvj.guannengcc.top

[R40] 追加写日志
来源：http://jpz.hesvh.cn

echo "log" >> out.log
来源：http://wys.cucudq.cn

[R41] 丢弃输出
来源：http://qfd.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://vgq.xuanzx.com

[R42] 输入重定向
来源：http://arb.zdbjq.cn

wc -l < a.txt
来源：http://wgg.epnwcf.com

[R43] 按名字查找文件
来源：http://tht.zhengqikj.top

find . -name "*.log" -type f
来源：http://ppk.ydjk.org.cn

[R44] 按修改时间查找
来源：http://tmu.sweek.top

find . -mtime -7 -type f
来源：http://bqf.gaohongyu789.top

[R45] 批量删除
来源：http://xnu.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://cnl.zycfv.cn

[R46] 递归替换文件内容
来源：http://ixh.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wwa.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://xit.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vtf.daria6918.cn

[R48] awk 取指定列
来源：http://ozk.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://cwo.yueranfly.top

[R49] awk 带条件
来源：http://uwt.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gfh.nwbrower.top

[R50] awk 求和
来源：http://lqf.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://xuu.hnxiangtu.top

[R51] 排序去重取前几
来源：http://wlp.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hqy.daria6918.cn

[R52] 统计行数
来源：http://tqp.fengsongda.top

wc -l a.txt
来源：http://gzm.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://nuo.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wbd.hfpthk.cn

[R54] 比较两个文件
来源：http://vfh.meibo888.top

diff a.txt b.txt
来源：http://hae.gotoacloud.top

[R55] 压缩与解压
来源：http://ukd.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulh.cqqwz.cn

[R56] 远程拷贝
来源：http://lhx.fzhhl.top

scp file user@host:/path/
来源：http://agz.9152youxi.cn

[R57] 远程执行命令
来源：http://hri.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://mcm.pycfn.com

[R58] 下载文件
来源：http://hrv.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mjf.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://stx.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jeq.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://udd.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vto.xuanzx.com

[R61] 磁盘占用
来源：http://pbr.birdmap.top

df -h;  du -sh *
来源：http://nxh.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://omw.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://wdq.aibaodan.cn

[R63] 内存与进程
来源：http://mzy.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://ijs.zdbjq.cn

[R64] 结束进程
来源：http://ebv.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://lhq.yj202588.top

[R65] 查看端口占用
来源：http://clg.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nvn.andypj.xyz

[R66] 定时任务
来源：http://hgi.hysaishi.cn

crontab -e;  crontab -l
来源：http://qiq.fengsongda.top

[R67] 生成随机十六进制串
来源：http://dgd.zhijiandao.cn

openssl rand -hex 16
来源：http://ttp.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://bhp.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://uwx.kuanghao11.cn

[R69] 生成随机密码
来源：http://qcq.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://nba.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://gdh.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://rbo.svipenyu.cn

[R71] 日期格式化
来源：http://pes.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nvo.ivvv.top

[R72] 等待端口就绪
来源：http://kjm.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wzu.jiagoushi.top

[R73] 分割大日志
来源：http://zns.cheryme.top

split -l 1000 big.log part_
来源：http://yro.daria6918.cn

[R74] 批量重命名
来源：http://ezy.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oar.jlsjyb.cn

[R75] 导出环境变量
来源：http://dku.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://gjk.zdbjq.cn

[R76] 使用临时文件
来源：http://isl.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://thy.chenlongwang.top

[R77] 读取用户输入
来源：http://sab.jyoumei.cn

read -rp "请输入: " ans
来源：http://mtk.jqgufenzy.top

[R78] 交互式菜单
来源：http://xtr.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ixo.yuxming.cn

[R79] 解析命令行选项
来源：http://hmb.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qjw.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://ugo.yfazqb.com

time ./run.sh
来源：http://meq.jinghuilouyu.cn

================================================================================
来源：http://pbf.zhijiandao.cn

S. C / C++ 专题
来源：http://bjx.yj20258.top

================================================================================
来源：http://isj.zhoulong.xyz

[S01] C：Hello World
来源：http://zne.c1oappe.top

#include <stdio.h>
来源：http://jix.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pkj.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://jsc.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://mtj.xuetiantiany.cn

[S03] C：读入整数
来源：http://nqy.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://opa.yueranfly.top

[S04] C：字符串复制
来源：http://now.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://jtp.yueranfly.top

[S05] C：字符串长度
来源：http://xbe.zdqjudy.top


<!-- 参考信息 -->