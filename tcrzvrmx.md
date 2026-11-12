代发 wailian999

[Q33] 多列分组
来源：http://ikl.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xrc.ppjwa.cn

[Q34] 每组取第一条
来源：http://jck.316326.xyz

SELECT * FROM (
来源：http://mfn.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hzh.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://rwl.c1oappe.top

[Q35] 内连接
来源：http://riz.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ctq.cheryme.top

[Q36] 左连接
来源：http://bdt.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bad.nanxuanxn.top

[Q37] 右连接
来源：http://odp.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfu.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://itt.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hxu.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://bjw.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://fgz.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ycr.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hqr.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aay.gogol.net.cn

[Q41] 多表连接
来源：http://opn.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ytz.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://iqm.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://tat.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://nup.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://oet.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bdo.52xcode.cn

[Q43] 标量子查询
来源：http://dlh.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://acg.nanxinkj.top

[Q44] IN 子查询
来源：http://fnx.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jvh.316326.xyz

[Q45] EXISTS 判断存在
来源：http://sjs.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibp.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://kau.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rkj.xziqi.cn

[Q47] 与平均值比较
来源：http://kon.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dok.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://kcj.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uvi.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://kyv.ybcxt.top

[Q49] 更新单行
来源：http://smt.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://asl.jqgufenzy.top

[Q50] 批量更新
来源：http://zwx.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iju.haohaochexian.top

[Q51] 用子查询更新
来源：http://hxo.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://osu.316326.xyz

[Q52] 删除指定行
来源：http://scg.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://kmq.smart0.xyz

[Q53] 按条件删除
来源：http://rqq.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://npa.jinghuilouyu.cn

[Q54] 清空表
来源：http://abd.yonumen.top

TRUNCATE TABLE logs;
来源：http://hij.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://tlt.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://viu.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://xmp.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://inm.fehbvm.com

[Q57] 行号
来源：http://uee.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ztw.meibo888.top

[Q58] 累计求和
来源：http://glk.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ltc.cqqwz.cn

[Q59] 分组内累计
来源：http://mnl.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://acu.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://zcl.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oei.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cki.mhx1999.top

[Q61] 移动平均
来源：http://auz.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yku.yfazqb.com

[Q62] 分组占比
来源：http://ebu.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://day.guannengcc.top

[Q63] 开启事务
来源：http://xyj.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hiu.pycfn.com

[Q64] 提交事务
来源：http://kgm.xingfuxueyuan.xyz

COMMIT;
来源：http://ynf.chenjidiqi.icu

[Q65] 回滚事务
来源：http://xok.tanke756.top

ROLLBACK;
来源：http://khc.dashuyun.cn

[Q66] 行锁查询
来源：http://opj.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://koh.jyoumei.cn

[Q67] 设置隔离级别
来源：http://pol.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cft.pycfn.com

[Q68] 保存点
来源：http://mcz.jinqigufen.top

SAVEPOINT sp1;
来源：http://wwu.epnwcf.com

ROLLBACK TO sp1;
来源：http://tqn.yanxiufei.cn

[Q69] 查看执行计划
来源：http://nsg.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qqb.zhongyouzk.top

[Q70] 更新统计信息
来源：http://bal.zhijiandao.cn

ANALYZE TABLE users;
来源：http://ewf.hesvh.cn

[Q71] 查看建表语句
来源：http://afv.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tob.daxiang520.top

[Q72] 查看索引
来源：http://lww.havefunace.top

SHOW INDEX FROM users;
来源：http://rnk.guannengcc.top

[Q73] 查看表状态
来源：http://zov.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zix.sufxvd.cn

[Q74] 强制使用索引
来源：http://ltl.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebh.xuanzx.com

[Q75] 日期格式化
来源：http://afc.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tnn.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dfi.vqdsnc.cn

[Q76] 按天统计
来源：http://fdk.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ezo.fanxiaobao.xyz

[Q77] 时间加减
来源：http://hcu.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jrh.chenlongwang.top

[Q78] 当前时间
来源：http://hib.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tqw.daxiang520.top

[Q79] 字符串拼接
来源：http://adh.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ndo.smart0.xyz

[Q80] 字符串截取
来源：http://pio.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tkj.c1oappe.top

[Q81] 字符串替换
来源：http://vay.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bxx.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://frv.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ljl.andypj.xyz

[Q83] 大小写转换
来源：http://xad.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://byt.zdbjq.cn

[Q84] 去除首尾空格
来源：http://uum.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://vpp.jyoumei.cn

[Q85] 数值取整
来源：http://jwj.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cgx.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://utm.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mho.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://zxy.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rft.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://cec.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vvw.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nht.havefunace.top

[Q89] 判断表是否存在
来源：http://sha.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dbg.sjlbkw.cn

[Q90] 生成序号列
来源：http://tyd.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://onr.316326.xyz

================================================================================
来源：http://pna.gzhubu.top

R. Bash 专题
来源：http://qaq.vqdsnc.cn

================================================================================
来源：http://hqb.ydzc1.top

[R01] shebang 与严格模式
来源：http://whz.smart0.xyz

#!/usr/bin/env bash
来源：http://zhq.cucudq.cn

set -euo pipefail
来源：http://dok.wangdashe.top

[R02] 变量赋值与使用
来源：http://oke.sysykeji.top

name="Tom"; echo "$name"
来源：http://szu.daria6918.cn

[R03] 只读变量
来源：http://htn.c1oappe.top

readonly PI=3.14
来源：http://dxn.hammf.cn

[R04] 位置参数
来源：http://enq.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nrj.sxryk.cn

[R05] 参数默认值
来源：http://xgj.yvedp.cn

name="${1:-default}"
来源：http://zla.chenlongwang.top

[R06] 判断命令是否存在
来源：http://ccm.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wnd.chenzaomai.com

[R07] if 判断文件
来源：http://glu.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ygj.yuanzhike.top

[R08] 数值比较
来源：http://iae.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://rzj.hywenlv.cn

[R09] 字符串比较
来源：http://bun.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jjw.yonumen.top

[R10] 正则匹配
来源：http://teb.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nxt.cqqwz.cn

[R11] case 多分支
来源：http://wte.yongpay.top

case "$1" in
来源：http://lwf.zycfv.cn

start) echo "启动" ;;
来源：http://nro.nanxinkj.top

stop)  echo "停止" ;;
来源：http://srq.bbcook.cn

*)     echo "未知命令" ;;
来源：http://ien.gogol.net.cn

esac
来源：http://qlk.jqgufenzy.top

[R12] for 遍历文件
来源：http://rbd.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://coy.hcnkem.com

[R13] for 计数循环
来源：http://bnk.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://bgu.tanke756.top

[R14] C 风格 for
来源：http://kfr.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ukb.dianchejie.cn

[R15] while 逐行读文件
来源：http://szg.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hfg.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://htx.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nzp.ybcxt.top

[R17] 数组定义与取值
来源：http://sml.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hde.yj20258.top

[R18] 遍历数组
来源：http://xti.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sfp.yvedp.cn

[R19] 数组长度
来源：http://vtu.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://npv.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://fof.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ofw.aibaodan.cn

[R21] 字符串长度
来源：http://qic.dashuyun.cn

echo "${#s}"
来源：http://wmv.iojbl.cn

[R22] 截取子串
来源：http://myn.hesvh.cn

echo "${s:0:5}"
来源：http://vfy.yj202588.top

[R23] 字符串替换
来源：http://aep.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ekq.yj20258888.top

[R24] 大小写转换
来源：http://ndo.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://pkl.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://oyw.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zkh.316326.xyz

[R26] 命令替换
来源：http://bzj.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://gft.gogol.net.cn

[R27] 算术展开
来源：http://qjc.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://pgg.shzxlz.cn

[R28] 浮点运算
来源：http://txx.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://igd.bjfxy.top

[R29] 定义函数
来源：http://kia.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iyt.kuanghao11.cn

[R30] 函数返回状态码
来源：http://rrf.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://ria.52xcode.cn

[R31] 局部变量
来源：http://xla.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://cmt.havefunace.top

[R32] 参数个数校验
来源：http://gfk.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://agv.cheryme.top

[R33] 捕获错误并提示行号
来源：http://knh.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rgi.chenjidiqi.icu

[R34] 退出时清理
来源：http://aqn.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://soo.nanxuanxn.top

[R35] 后台执行并等待
来源：http://avn.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://exf.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://vti.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vxv.yj20258888.top

[R37] 把输出赋给变量
来源：http://gtk.mhx1999.top

files=$(ls -1)
来源：http://cfw.zhengqikj.top

[R38] 管道串联
来源：http://tvw.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://lch.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://biq.hcnkem.com

cmd > out.log 2>&1
来源：http://vtp.cheryme.top

[R40] 追加写日志
来源：http://jtx.xziqi.cn

echo "log" >> out.log
来源：http://exe.yangfankeji.com

[R41] 丢弃输出
来源：http://qbq.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://mcg.jqgufenzy.top

[R42] 输入重定向
来源：http://ord.bjfxy.top

wc -l < a.txt
来源：http://gci.jlsjyb.cn

[R43] 按名字查找文件
来源：http://qid.hfpthk.cn

find . -name "*.log" -type f
来源：http://cwy.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://ugb.zhoulong.xyz

find . -mtime -7 -type f
来源：http://lzm.hfpthk.cn

[R45] 批量删除
来源：http://uqh.sysykeji.top

find . -name "*.tmp" -delete
来源：http://ftw.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://cbb.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://adh.guowangkeji.top

[R47] sed 单行替换
来源：http://cha.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wak.gaohongyu789.top

[R48] awk 取指定列
来源：http://ory.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://ifm.dianchejie.cn

[R49] awk 带条件
来源：http://bfq.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxz.jinyuanbaomall.cn

[R50] awk 求和
来源：http://cmz.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://qjn.zhoulong.xyz

[R51] 排序去重取前几
来源：http://opd.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xus.chenzaomai.com

[R52] 统计行数
来源：http://yok.iojbl.cn

wc -l a.txt
来源：http://zku.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://cxi.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://snt.ydjk.org.cn

[R54] 比较两个文件
来源：http://dbj.cucudq.cn

diff a.txt b.txt
来源：http://whe.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://npi.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wyh.sxryk.cn

[R56] 远程拷贝
来源：http://lfn.cdnleiting.top

scp file user@host:/path/
来源：http://jqz.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://tfz.andypj.xyz

ssh user@host 'uptime'
来源：http://xsy.feifeiyinyue.top

[R58] 下载文件
来源：http://szn.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://udo.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://jyv.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mtl.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://sim.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qfn.yueranfly.top

[R61] 磁盘占用
来源：http://bbq.jlsjyb.cn

df -h;  du -sh *
来源：http://zte.chenzaomai.com

[R62] 找最占空间的文件
来源：http://szm.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://hzv.dianchejie.cn

[R63] 内存与进程
来源：http://aso.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://yrm.chenjidiqi.icu

[R64] 结束进程
来源：http://skn.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://mat.epnwcf.com

[R65] 查看端口占用
来源：http://kde.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ioy.316326.xyz

[R66] 定时任务
来源：http://chr.yfazqb.com

crontab -e;  crontab -l
来源：http://ibz.iojbl.cn

[R67] 生成随机十六进制串
来源：http://ica.kuanghao11.cn

openssl rand -hex 16
来源：http://huw.vehdjk.com

[R68] 计算文件校验值
来源：http://tff.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mho.nanxuanxn.top

[R69] 生成随机密码
来源：http://kek.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://xpu.quarkkingdee.top

[R70] 时间戳与互转
来源：http://qmu.sysykeji.top

date +%s;  date -d @1700000000
来源：http://jbh.chenjidiqi.icu

[R71] 日期格式化
来源：http://jjt.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://vwm.gogol.net.cn

[R72] 等待端口就绪
来源：http://vmu.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fvc.yfazqb.com

[R73] 分割大日志
来源：http://vmr.guowangkeji.top

split -l 1000 big.log part_
来源：http://dmy.nanxinkj.top

[R74] 批量重命名
来源：http://kin.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://btn.redwolf501.top

[R75] 导出环境变量
来源：http://jqd.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://kmu.zhongyouzk.top

[R76] 使用临时文件
来源：http://ozt.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dqd.yfazqb.com

[R77] 读取用户输入
来源：http://jel.chenlongwang.top

read -rp "请输入: " ans
来源：http://vys.zycfv.cn

[R78] 交互式菜单
来源：http://kvn.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://olb.yonumen.top

[R79] 解析命令行选项
来源：http://yfv.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twk.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://zbf.xylfe.cn

time ./run.sh
来源：http://gac.hywenlv.cn

================================================================================
来源：http://zny.daria6918.cn

S. C / C++ 专题
来源：http://kza.ydjk.org.cn

================================================================================
来源：http://pei.nanxinkj.top

[S01] C：Hello World
来源：http://shz.hongshengwenyu.top

#include <stdio.h>
来源：http://cev.sxryk.cn


<!-- 参考信息 -->