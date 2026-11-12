代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pod.ydzc1.top

) t WHERE rn = 1;
来源：http://emr.havefunace.top

[Q35] 内连接
来源：http://nja.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ckl.sxryk.cn

[Q36] 左连接
来源：http://grx.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sfq.feifeiyinyue.top

[Q37] 右连接
来源：http://xvr.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ans.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wvg.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lmk.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://lfp.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://azy.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://alg.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lrf.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gvr.hcnkem.com

[Q41] 多表连接
来源：http://lvr.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ajp.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://jsi.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://oyx.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://nuc.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://mob.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sbd.yangfankeji.com

[Q43] 标量子查询
来源：http://mel.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jsj.c1oappe.top

[Q44] IN 子查询
来源：http://fwf.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kkv.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://ynd.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wen.nanxinkj.top

[Q46] NOT EXISTS 判断不存在
来源：http://cht.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mlg.gaohongyu789.top

[Q47] 与平均值比较
来源：http://spx.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lom.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://xyy.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dat.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://jav.yangfankeji.com

[Q49] 更新单行
来源：http://rfq.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tqc.yj20258.top

[Q50] 批量更新
来源：http://dlq.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ldm.ybcxt.top

[Q51] 用子查询更新
来源：http://oog.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ate.xziqi.cn

[Q52] 删除指定行
来源：http://lpp.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://egz.zhoulong.xyz

[Q53] 按条件删除
来源：http://abw.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xte.guannengcc.top

[Q54] 清空表
来源：http://qzf.bbcook.cn

TRUNCATE TABLE logs;
来源：http://rdx.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://jdu.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aft.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://boq.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jkx.wangdashe.top

[Q57] 行号
来源：http://vtm.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eyj.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://ydr.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://taq.sufxvd.cn

[Q59] 分组内累计
来源：http://lmm.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nmy.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://wqk.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gjs.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zpw.shzxlz.cn

[Q61] 移动平均
来源：http://joe.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ely.kuanghao11.cn

[Q62] 分组占比
来源：http://prx.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxp.snrcjt.cn

[Q63] 开启事务
来源：http://eej.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ciu.birdmap.top

[Q64] 提交事务
来源：http://paj.xuanzx.com

COMMIT;
来源：http://hxx.tarul.cn

[Q65] 回滚事务
来源：http://tgt.yangfankeji.com

ROLLBACK;
来源：http://skh.yuxming.cn

[Q66] 行锁查询
来源：http://fly.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gdy.cucudq.cn

[Q67] 设置隔离级别
来源：http://jkg.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tqr.aibaodan.cn

[Q68] 保存点
来源：http://fyb.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://rqi.mhx1999.top

ROLLBACK TO sp1;
来源：http://wuv.ybcxt.top

[Q69] 查看执行计划
来源：http://nxc.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ldy.haohaochexian.top

[Q70] 更新统计信息
来源：http://lht.xuanzx.com

ANALYZE TABLE users;
来源：http://fvn.aibaodan.cn

[Q71] 查看建表语句
来源：http://bbg.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qfj.cashguo.top

[Q72] 查看索引
来源：http://txv.sxryk.cn

SHOW INDEX FROM users;
来源：http://lew.fengsongda.top

[Q73] 查看表状态
来源：http://obl.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://jok.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://sfl.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dfh.ybcxt.top

[Q75] 日期格式化
来源：http://mrl.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://inu.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vmj.shangyingyoupin.top

[Q76] 按天统计
来源：http://dfl.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://equ.dianchejie.cn

[Q77] 时间加减
来源：http://pdp.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fcd.shangyingyoupin.top

[Q78] 当前时间
来源：http://wse.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lmp.nwbrower.top

[Q79] 字符串拼接
来源：http://stc.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://let.xylfe.cn

[Q80] 字符串截取
来源：http://yqc.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hle.wangshuangyany.cn

[Q81] 字符串替换
来源：http://ewt.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baq.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://jnl.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rqd.gotoacloud.top

[Q83] 大小写转换
来源：http://iuj.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eyi.bjfxy.top

[Q84] 去除首尾空格
来源：http://emm.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://cgr.shzxlz.cn

[Q85] 数值取整
来源：http://coj.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qkb.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://ihj.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dmd.wangdashe.top

[Q87] JSON 字段做条件
来源：http://rjf.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rte.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://ymx.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dvy.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xmt.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://hjb.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rtb.daxiang520.top

[Q90] 生成序号列
来源：http://owh.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mdg.fktsv.cn

================================================================================
来源：http://umw.nanxinkj.top

R. Bash 专题
来源：http://gea.cheryme.top

================================================================================
来源：http://idi.hammf.cn

[R01] shebang 与严格模式
来源：http://baf.tian-w.cn

#!/usr/bin/env bash
来源：http://eqv.0kj1m.cn

set -euo pipefail
来源：http://ich.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://sjs.xziqi.cn

name="Tom"; echo "$name"
来源：http://cmq.zdqjudy.top

[R03] 只读变量
来源：http://fmn.yongpay.top

readonly PI=3.14
来源：http://ufq.yangfankeji.com

[R04] 位置参数
来源：http://lhm.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rbo.9152youxi.cn

[R05] 参数默认值
来源：http://cpz.jianghu66.top

name="${1:-default}"
来源：http://vbb.zdqjudy.top

[R06] 判断命令是否存在
来源：http://kqy.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ehc.yongpay.top

[R07] if 判断文件
来源：http://rux.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wof.bbcook.cn

[R08] 数值比较
来源：http://dir.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jsc.tanke756.top

[R09] 字符串比较
来源：http://url.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xac.ivvv.top

[R10] 正则匹配
来源：http://kph.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrb.mhx1999.top

[R11] case 多分支
来源：http://cow.52xcode.cn

case "$1" in
来源：http://kmj.hfpthk.cn

start) echo "启动" ;;
来源：http://avh.zdbjq.cn

stop)  echo "停止" ;;
来源：http://ieg.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://ohz.yonumen.top

esac
来源：http://ven.ppjwa.cn

[R12] for 遍历文件
来源：http://oby.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://ifa.hnxiangtu.top

[R13] for 计数循环
来源：http://swa.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://wsa.gzhubu.top

[R14] C 风格 for
来源：http://she.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nrt.fehbvm.com

[R15] while 逐行读文件
来源：http://eal.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awe.ppjwa.cn

[R16] until 等待条件
来源：http://bfx.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jlr.xziqi.cn

[R17] 数组定义与取值
来源：http://tum.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://byq.fzhhl.top

[R18] 遍历数组
来源：http://nnp.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ytb.xuetiantiany.cn

[R19] 数组长度
来源：http://sfu.jyoumei.cn

echo "${#arr[@]}"
来源：http://vno.sufxvd.cn

[R20] 关联数组（字典）
来源：http://tfg.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bkz.yj202588.top

[R21] 字符串长度
来源：http://imn.yvedp.cn

echo "${#s}"
来源：http://tuj.jiagoushi.top

[R22] 截取子串
来源：http://eay.vehdjk.com

echo "${s:0:5}"
来源：http://phj.ppjwa.cn

[R23] 字符串替换
来源：http://ejd.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://enw.vqdsnc.cn

[R24] 大小写转换
来源：http://hyz.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bje.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://viz.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fhk.iojbl.cn

[R26] 命令替换
来源：http://qlh.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://ynp.andypj.xyz

[R27] 算术展开
来源：http://zvv.ydzc1.top

echo $((1 + 2 * 3))
来源：http://vna.daxiang520.top

[R28] 浮点运算
来源：http://kzd.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://hbq.zhiwuduotai.top

[R29] 定义函数
来源：http://vzc.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hie.pycfn.com

[R30] 函数返回状态码
来源：http://ppx.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://eym.wangshuangyany.cn

[R31] 局部变量
来源：http://rku.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://opv.hesvh.cn

[R32] 参数个数校验
来源：http://vez.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vmh.cheryme.top

[R33] 捕获错误并提示行号
来源：http://ubp.zhaomingkeji.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dgq.jinqigufen.top

[R34] 退出时清理
来源：http://yvr.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hvw.aibaodan.cn

[R35] 后台执行并等待
来源：http://aqn.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lff.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://gcv.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://trf.jinqigufen.top

[R37] 把输出赋给变量
来源：http://sov.svipenyu.cn

files=$(ls -1)
来源：http://llu.pycfn.com

[R38] 管道串联
来源：http://nog.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://qlw.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://chf.9152youxi.cn

cmd > out.log 2>&1
来源：http://jdf.ppjwa.cn

[R40] 追加写日志
来源：http://ryw.tanke756.top

echo "log" >> out.log
来源：http://rdu.xinyue.icu

[R41] 丢弃输出
来源：http://pjx.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://rdv.52xcode.cn

[R42] 输入重定向
来源：http://rpy.smart0.xyz

wc -l < a.txt
来源：http://eam.chenzaomai.com

[R43] 按名字查找文件
来源：http://evi.hysaishi.cn

find . -name "*.log" -type f
来源：http://spi.uphjek.com

[R44] 按修改时间查找
来源：http://cfz.zhijiandao.cn

find . -mtime -7 -type f
来源：http://uoj.nwbrower.top

[R45] 批量删除
来源：http://sbz.tian-w.cn

find . -name "*.tmp" -delete
来源：http://ydv.xylfe.cn

[R46] 递归替换文件内容
来源：http://jqi.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uxv.yuanzhike.top

[R47] sed 单行替换
来源：http://lax.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://itq.jinqigfzy.top

[R48] awk 取指定列
来源：http://lhj.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://aps.sweek.top

[R49] awk 带条件
来源：http://ybc.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pnq.jlsjyb.cn

[R50] awk 求和
来源：http://ita.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://bfv.ydzc1.top

[R51] 排序去重取前几
来源：http://bzd.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yeo.zhongyouzk.top

[R52] 统计行数
来源：http://pfr.gogol.net.cn

wc -l a.txt
来源：http://nwk.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://lsn.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mfq.ppjwa.cn

[R54] 比较两个文件
来源：http://zhh.dashuyun.cn

diff a.txt b.txt
来源：http://lqj.xuanzx.com

[R55] 压缩与解压
来源：http://hqt.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ewh.zhixingplan.top

[R56] 远程拷贝
来源：http://eek.jqgufenzy.top

scp file user@host:/path/
来源：http://khz.tanke756.top

[R57] 远程执行命令
来源：http://gqe.316326.xyz

ssh user@host 'uptime'
来源：http://xhb.hnxiangtu.top

[R58] 下载文件
来源：http://tcx.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mqi.ybcxt.top

[R59] 发 POST JSON
来源：http://yqe.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zbl.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://pxr.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bai.zhiwuduotai.top

[R61] 磁盘占用
来源：http://cva.52xcode.cn

df -h;  du -sh *
来源：http://osk.tianlin.xyz

[R62] 找最占空间的文件
来源：http://ier.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://zcg.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://lki.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://loh.aizwys.cn

[R64] 结束进程
来源：http://ptg.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://gih.cqqwz.cn

[R65] 查看端口占用
来源：http://hms.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iyi.sxryk.cn

[R66] 定时任务
来源：http://emn.xinyue.icu

crontab -e;  crontab -l
来源：http://uep.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://ryf.snrcjt.cn

openssl rand -hex 16
来源：http://nsl.jiagoushi.top

[R68] 计算文件校验值
来源：http://ort.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://odm.andypj.xyz

[R69] 生成随机密码
来源：http://smj.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://pyy.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ixt.xinyue.icu

date +%s;  date -d @1700000000
来源：http://ztb.svipenyu.cn

[R71] 日期格式化
来源：http://fiu.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ban.yonumen.top

[R72] 等待端口就绪
来源：http://mtt.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://khc.bjfxy.top

[R73] 分割大日志
来源：http://rqf.snrcjt.cn

split -l 1000 big.log part_
来源：http://dbg.iojbl.cn

[R74] 批量重命名
来源：http://tvg.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tpm.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://lwu.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://msy.yueranfly.top

[R76] 使用临时文件
来源：http://kjw.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kac.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://oza.jlsjyb.cn

read -rp "请输入: " ans
来源：http://tst.zhixingplan.top

[R78] 交互式菜单
来源：http://vit.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ong.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://fhq.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yvh.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://mit.xinyue.icu

time ./run.sh
来源：http://aol.havefunace.top

================================================================================
来源：http://wlk.xinyue.icu

S. C / C++ 专题
来源：http://kig.sweek.top

================================================================================
来源：http://dad.svipenyu.cn

[S01] C：Hello World
来源：http://vsx.316326.xyz

#include <stdio.h>
来源：http://xqh.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qnj.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://bae.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://hwl.hywenlv.cn

[S03] C：读入整数
来源：http://oyk.jyoumei.cn


<!-- 参考信息 -->