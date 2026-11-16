代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://bcy.uphjek.com

[Q30] 分组统计
来源：http://upo.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndu.yvedp.cn

[Q31] 分组后过滤
来源：http://orv.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yjy.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://fjf.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugw.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bcl.quarkkingdee.top

[Q33] 多列分组
来源：http://qyo.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xos.yj202588.top

[Q34] 每组取第一条
来源：http://fli.hysaishi.cn

SELECT * FROM (
来源：http://fet.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kbx.ivvv.top

) t WHERE rn = 1;
来源：http://ocs.wangshuangyany.cn

[Q35] 内连接
来源：http://wce.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qee.jlsjyb.cn

[Q36] 左连接
来源：http://bge.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://glz.jinqigufen.top

[Q37] 右连接
来源：http://bvi.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oex.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://zrm.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uyi.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://dww.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uvl.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hnm.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://esr.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zsm.jqgfzy.top

[Q41] 多表连接
来源：http://npt.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yzu.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://tlc.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://drn.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://rne.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://coo.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://azl.316326.xyz

[Q43] 标量子查询
来源：http://kkb.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mtv.hywenlv.cn

[Q44] IN 子查询
来源：http://fhb.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dju.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://bea.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqw.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://buv.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tdj.fehbvm.com

[Q47] 与平均值比较
来源：http://nng.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qle.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://dhm.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mek.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://imn.xziqi.cn

[Q49] 更新单行
来源：http://mzo.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eah.snrcjt.cn

[Q50] 批量更新
来源：http://dpl.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vfs.tian-w.cn

[Q51] 用子查询更新
来源：http://yrc.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iys.yuxming.cn

[Q52] 删除指定行
来源：http://wzg.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://egq.hammf.cn

[Q53] 按条件删除
来源：http://yfb.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sem.sweek.top

[Q54] 清空表
来源：http://yyl.havefunace.top

TRUNCATE TABLE logs;
来源：http://nct.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://hlo.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://grd.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://caz.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dkg.yonumen.top

[Q57] 行号
来源：http://tif.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uzf.ivvv.top

[Q58] 累计求和
来源：http://hyr.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ivh.chenjidiqi.icu

[Q59] 分组内累计
来源：http://rxb.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rxy.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://lcb.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pmf.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zcc.snrcjt.cn

[Q61] 移动平均
来源：http://anb.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lkl.gzhubu.top

[Q62] 分组占比
来源：http://bao.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xac.jiagoushi.top

[Q63] 开启事务
来源：http://lzs.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ayj.ehwqpu.com

[Q64] 提交事务
来源：http://fgc.yuanzhike.top

COMMIT;
来源：http://joz.dianchejie.cn

[Q65] 回滚事务
来源：http://usg.0kj1m.cn

ROLLBACK;
来源：http://rkq.gzhubu.top

[Q66] 行锁查询
来源：http://vin.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://igi.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://ouh.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ujs.pengpengdd.cyou

[Q68] 保存点
来源：http://wyq.tanke756.top

SAVEPOINT sp1;
来源：http://rby.nwbrower.top

ROLLBACK TO sp1;
来源：http://ywm.cdnleiting.top

[Q69] 查看执行计划
来源：http://cpd.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://geh.birdmap.top

[Q70] 更新统计信息
来源：http://por.xziqi.cn

ANALYZE TABLE users;
来源：http://lux.jqgufenzy.top

[Q71] 查看建表语句
来源：http://jdd.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mnu.wangshuangyany.cn

[Q72] 查看索引
来源：http://amo.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://rjy.wangdashe.top

[Q73] 查看表状态
来源：http://ovc.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://krn.fehbvm.com

[Q74] 强制使用索引
来源：http://xbh.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kdw.tian-w.cn

[Q75] 日期格式化
来源：http://oyw.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zvj.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eeq.xuanzx.com

[Q76] 按天统计
来源：http://ahj.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nik.shzxlz.cn

[Q77] 时间加减
来源：http://jwg.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qfr.pycfn.com

[Q78] 当前时间
来源：http://qhd.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bbr.haohaochexian.top

[Q79] 字符串拼接
来源：http://jqp.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehk.hywenlv.cn

[Q80] 字符串截取
来源：http://fks.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xgc.zycfv.cn

[Q81] 字符串替换
来源：http://hvo.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lla.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://gow.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xdy.haohaochexian.top

[Q83] 大小写转换
来源：http://ndu.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jzr.xinyue.icu

[Q84] 去除首尾空格
来源：http://etl.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://jem.hywenlv.cn

[Q85] 数值取整
来源：http://lpd.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ebu.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://kvj.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hyr.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://bbc.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bgr.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://gtw.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uxv.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uzr.havefunace.top

[Q89] 判断表是否存在
来源：http://igw.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yjk.cashguo.top

[Q90] 生成序号列
来源：http://per.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hlq.bjfxy.top

================================================================================
来源：http://inr.aibaodan.cn

R. Bash 专题
来源：http://ccs.316326.xyz

================================================================================
来源：http://wlj.ppjwa.cn

[R01] shebang 与严格模式
来源：http://zht.ehwqpu.com

#!/usr/bin/env bash
来源：http://xlw.sysykeji.top

set -euo pipefail
来源：http://arq.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://pox.nanxinkj.top

name="Tom"; echo "$name"
来源：http://yqe.yuxming.cn

[R03] 只读变量
来源：http://jbg.fehbvm.com

readonly PI=3.14
来源：http://wou.xylfe.cn

[R04] 位置参数
来源：http://gtm.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tls.fzhhl.top

[R05] 参数默认值
来源：http://low.yanxiufei.cn

name="${1:-default}"
来源：http://pgn.fengsongda.top

[R06] 判断命令是否存在
来源：http://fsf.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsp.tanke756.top

[R07] if 判断文件
来源：http://vpc.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhj.chenlongwang.top

[R08] 数值比较
来源：http://awv.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rbh.yongpay.top

[R09] 字符串比较
来源：http://bjv.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nhj.zdbjq.cn

[R10] 正则匹配
来源：http://gqz.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ytw.dashuyun.cn

[R11] case 多分支
来源：http://jwp.zhiwuduotai.top

case "$1" in
来源：http://bcv.guowangkeji.top

start) echo "启动" ;;
来源：http://dcz.wangdashe.top

stop)  echo "停止" ;;
来源：http://vdh.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://okm.fanxiaobao.xyz

esac
来源：http://pgz.tanke756.top

[R12] for 遍历文件
来源：http://vae.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://gjm.mhx1999.top

[R13] for 计数循环
来源：http://vzw.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qcz.aibaodan.cn

[R14] C 风格 for
来源：http://huy.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ekb.jiagoushi.top

[R15] while 逐行读文件
来源：http://xux.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlf.daria6918.cn

[R16] until 等待条件
来源：http://asm.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fok.sjlbkw.cn

[R17] 数组定义与取值
来源：http://idx.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://coa.nanxuanxn.top

[R18] 遍历数组
来源：http://ham.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wvn.iojbl.cn

[R19] 数组长度
来源：http://knu.jqgfzy.top

echo "${#arr[@]}"
来源：http://szq.fzhhl.top

[R20] 关联数组（字典）
来源：http://wsu.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://epr.bbcook.cn

[R21] 字符串长度
来源：http://nry.shuidangran.top

echo "${#s}"
来源：http://kmr.sxryk.cn

[R22] 截取子串
来源：http://yra.haohaochexian.top

echo "${s:0:5}"
来源：http://jjf.hfpthk.cn

[R23] 字符串替换
来源：http://xtl.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jub.nanxinkj.top

[R24] 大小写转换
来源：http://rpp.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zwf.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://wgi.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jya.yvedp.cn

[R26] 命令替换
来源：http://pov.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://yxh.hammf.cn

[R27] 算术展开
来源：http://xmo.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://mfh.c1oappe.top

[R28] 浮点运算
来源：http://jsi.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://jns.fehbvm.com

[R29] 定义函数
来源：http://cnf.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wtg.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://mzq.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://xxf.svipenyu.cn

[R31] 局部变量
来源：http://xbn.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://tob.ydzc1.top

[R32] 参数个数校验
来源：http://msn.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rin.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ejj.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kac.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://zjf.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rpc.sxryk.cn

[R35] 后台执行并等待
来源：http://fyk.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aux.daxiang520.top

[R36] 并发执行多个任务
来源：http://emk.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mxj.sufxvd.cn

[R37] 把输出赋给变量
来源：http://shs.yonumen.top

files=$(ls -1)
来源：http://ymy.fanxiaobao.xyz

[R38] 管道串联
来源：http://dss.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://yix.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://zdk.uphjek.com

cmd > out.log 2>&1
来源：http://kwm.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://ete.gogol.net.cn

echo "log" >> out.log
来源：http://ikf.hesvh.cn

[R41] 丢弃输出
来源：http://qms.iojbl.cn

cmd >/dev/null 2>&1
来源：http://gxm.birdmap.top

[R42] 输入重定向
来源：http://sxh.tian-w.cn

wc -l < a.txt
来源：http://wja.sysykeji.top

[R43] 按名字查找文件
来源：http://ofu.nanxinkj.top

find . -name "*.log" -type f
来源：http://qgp.c1oappe.top

[R44] 按修改时间查找
来源：http://rpv.shzxlz.cn

find . -mtime -7 -type f
来源：http://rst.gotoacloud.top

[R45] 批量删除
来源：http://bbx.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://afx.yuanzhike.top

[R46] 递归替换文件内容
来源：http://rcx.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://olz.zhiwuduotai.top

[R47] sed 单行替换
来源：http://enh.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://jkf.aibaodan.cn

[R48] awk 取指定列
来源：http://zsm.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://frk.9152youxi.cn

[R49] awk 带条件
来源：http://uxo.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oda.smart0.xyz

[R50] awk 求和
来源：http://tmp.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wnl.jinqigfzy.top

[R51] 排序去重取前几
来源：http://htm.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lan.chenlongwang.top

[R52] 统计行数
来源：http://gtk.tian-w.cn

wc -l a.txt
来源：http://nqc.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://crm.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jhd.aibaodan.cn

[R54] 比较两个文件
来源：http://fiy.yj202588.top

diff a.txt b.txt
来源：http://qyp.xuetiantiany.cn

[R55] 压缩与解压
来源：http://ajz.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://trd.yuxming.cn

[R56] 远程拷贝
来源：http://khi.sjlbkw.cn

scp file user@host:/path/
来源：http://dne.jqgufenzy.top

[R57] 远程执行命令
来源：http://zrg.iojbl.cn

ssh user@host 'uptime'
来源：http://mnj.shzxlz.cn

[R58] 下载文件
来源：http://fjl.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rrt.sysykeji.top

[R59] 发 POST JSON
来源：http://ivs.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ftp.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://lpv.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zdp.birdmap.top

[R61] 磁盘占用
来源：http://uho.epnwcf.com

df -h;  du -sh *
来源：http://cue.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://wjv.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://zeh.jinqigufen.top

[R63] 内存与进程
来源：http://lbi.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://nqg.meibo888.top

[R64] 结束进程
来源：http://fxx.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://zhx.cdnleiting.top

[R65] 查看端口占用
来源：http://xzd.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kqv.yuanzhike.top

[R66] 定时任务
来源：http://ury.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://jgc.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://xoe.pycfn.com

openssl rand -hex 16
来源：http://xie.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://tss.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hwn.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://lxt.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://mho.sweek.top

[R70] 时间戳与互转
来源：http://dnj.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://qns.jinqigfzy.top

[R71] 日期格式化
来源：http://dzj.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eky.wangdashe.top

[R72] 等待端口就绪
来源：http://cay.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ujg.aizwys.cn

[R73] 分割大日志
来源：http://dwx.yongpay.top

split -l 1000 big.log part_
来源：http://kgv.cucudq.cn

[R74] 批量重命名
来源：http://jsw.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kfy.52xcode.cn

[R75] 导出环境变量
来源：http://ibr.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://ohv.haohaochexian.top

[R76] 使用临时文件
来源：http://sxz.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gif.cqqwz.cn

[R77] 读取用户输入
来源：http://rgv.xinyue.icu

read -rp "请输入: " ans
来源：http://oem.shuidangran.top

[R78] 交互式菜单
来源：http://ijd.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hzy.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://kwz.meibo888.top


<!-- 参考信息 -->