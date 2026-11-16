代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vke.daria6918.cn

[Q32] 分组拼接字符串
来源：http://oxa.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wuk.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bpo.epnwcf.com

[Q33] 多列分组
来源：http://cpq.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vgo.yj20258888.top

[Q34] 每组取第一条
来源：http://bqm.jinghuilouyu.cn

SELECT * FROM (
来源：http://eos.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nid.hnqzz.top

) t WHERE rn = 1;
来源：http://lyi.havefunace.top

[Q35] 内连接
来源：http://jvi.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iua.zhongyouzk.top

[Q36] 左连接
来源：http://nit.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://azr.316326.xyz

[Q37] 右连接
来源：http://tym.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uiz.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ylf.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yqs.tarul.cn

[Q39] 自连接（查上下级）
来源：http://zzc.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ori.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hnr.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ijw.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fku.dashuyun.cn

[Q41] 多表连接
来源：http://hch.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uvu.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://otq.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://apu.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://qli.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://aol.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwr.jyoumei.cn

[Q43] 标量子查询
来源：http://iza.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rpg.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://urh.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eub.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://cwq.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kru.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://iot.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sie.yangfankeji.com

[Q47] 与平均值比较
来源：http://cxw.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://koi.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://jgh.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aum.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://xbm.uphjek.com

[Q49] 更新单行
来源：http://hti.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rwe.hysaishi.cn

[Q50] 批量更新
来源：http://cdh.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfz.gzhubu.top

[Q51] 用子查询更新
来源：http://ybc.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://msl.aibaodan.cn

[Q52] 删除指定行
来源：http://ecq.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://apj.xylfe.cn

[Q53] 按条件删除
来源：http://wfp.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gvd.yueranfly.top

[Q54] 清空表
来源：http://skl.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://tmu.tanke756.top

[Q55] 排名（并列占位）
来源：http://rvc.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hxs.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://zos.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gwt.jiagoushi.top

[Q57] 行号
来源：http://qgi.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iso.tanke756.top

[Q58] 累计求和
来源：http://qap.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tza.gogol.net.cn

[Q59] 分组内累计
来源：http://sjr.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mxe.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://ukj.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zel.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://atz.sjlbkw.cn

[Q61] 移动平均
来源：http://ntn.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://foq.ivvv.top

[Q62] 分组占比
来源：http://sxn.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ozl.wangdashe.top

[Q63] 开启事务
来源：http://oaj.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ajm.tianlin.xyz

[Q64] 提交事务
来源：http://cmn.yueranfly.top

COMMIT;
来源：http://ruu.sxryk.cn

[Q65] 回滚事务
来源：http://rhg.zhengqikj.top

ROLLBACK;
来源：http://sks.fzhhl.top

[Q66] 行锁查询
来源：http://isl.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sjt.jiagoushi.top

[Q67] 设置隔离级别
来源：http://nll.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zko.yj20258888.top

[Q68] 保存点
来源：http://cpk.yueranfly.top

SAVEPOINT sp1;
来源：http://toz.shuidangran.top

ROLLBACK TO sp1;
来源：http://dyh.yuanzhike.top

[Q69] 查看执行计划
来源：http://gug.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xsh.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://ymb.jqgfzy.top

ANALYZE TABLE users;
来源：http://nxh.zhongyouzk.top

[Q71] 查看建表语句
来源：http://wch.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ujc.hammf.cn

[Q72] 查看索引
来源：http://qya.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://zak.jianghu66.top

[Q73] 查看表状态
来源：http://aga.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xpf.guowangkeji.top

[Q74] 强制使用索引
来源：http://vzu.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zzb.daxiang520.top

[Q75] 日期格式化
来源：http://ujj.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mbp.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jrw.yanxiufei.cn

[Q76] 按天统计
来源：http://oic.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nta.gogol.net.cn

[Q77] 时间加减
来源：http://nmb.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://acx.shzxlz.cn

[Q78] 当前时间
来源：http://lzs.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pwy.hcnkem.com

[Q79] 字符串拼接
来源：http://yju.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nkr.zdqjudy.top

[Q80] 字符串截取
来源：http://vbe.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ahc.ybcxt.top

[Q81] 字符串替换
来源：http://vzd.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zgm.tarul.cn

[Q82] 字符长度与字节长度
来源：http://xhs.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://phm.jlsjyb.cn

[Q83] 大小写转换
来源：http://qxs.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://twy.cheryme.top

[Q84] 去除首尾空格
来源：http://hoz.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://bfx.dashuyun.cn

[Q85] 数值取整
来源：http://eye.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zsq.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://fls.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fgn.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://qds.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gjz.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://yxj.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ajl.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kcv.nanxinkj.top

[Q89] 判断表是否存在
来源：http://xzn.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwa.fktsv.cn

[Q90] 生成序号列
来源：http://epe.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sod.cashguo.top

================================================================================
来源：http://ezg.haohaochexian.top

R. Bash 专题
来源：http://wgo.hywenlv.cn

================================================================================
来源：http://snh.snrcjt.cn

[R01] shebang 与严格模式
来源：http://zhk.hnqzz.top

#!/usr/bin/env bash
来源：http://xqf.quarkkingdee.top

set -euo pipefail
来源：http://hee.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://mag.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://cte.yfazqb.com

[R03] 只读变量
来源：http://ohi.hnqzz.top

readonly PI=3.14
来源：http://iii.xuetiantiany.cn

[R04] 位置参数
来源：http://upv.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tbb.wangshuangyany.cn

[R05] 参数默认值
来源：http://ezy.kuanghao11.cn

name="${1:-default}"
来源：http://qje.smart0.xyz

[R06] 判断命令是否存在
来源：http://wcq.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ava.jlsjyb.cn

[R07] if 判断文件
来源：http://qnc.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dny.zhijiandao.cn

[R08] 数值比较
来源：http://ibt.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pzt.9152youxi.cn

[R09] 字符串比较
来源：http://qqs.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bej.wangshuangyany.cn

[R10] 正则匹配
来源：http://ycg.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nvd.tianlin.xyz

[R11] case 多分支
来源：http://svq.guannengcc.top

case "$1" in
来源：http://odr.andypj.xyz

start) echo "启动" ;;
来源：http://tke.havefunace.top

stop)  echo "停止" ;;
来源：http://nmd.bbcook.cn

*)     echo "未知命令" ;;
来源：http://rth.svipenyu.cn

esac
来源：http://tgt.hammf.cn

[R12] for 遍历文件
来源：http://mlh.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://zdt.snrcjt.cn

[R13] for 计数循环
来源：http://wup.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://jqs.uphjek.com

[R14] C 风格 for
来源：http://dqu.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bih.snrcjt.cn

[R15] while 逐行读文件
来源：http://fpy.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pyw.ctjpmb.com

[R16] until 等待条件
来源：http://mvn.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qcj.sufxvd.cn

[R17] 数组定义与取值
来源：http://eku.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://lhs.shanyushiyangtech.top

[R18] 遍历数组
来源：http://bul.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ouy.hysaishi.cn

[R19] 数组长度
来源：http://upo.0kj1m.cn

echo "${#arr[@]}"
来源：http://bte.sysykeji.top

[R20] 关联数组（字典）
来源：http://dzi.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uko.nanxuanxn.top

[R21] 字符串长度
来源：http://tjg.zhiwuduotai.top

echo "${#s}"
来源：http://xud.nanxinkj.top

[R22] 截取子串
来源：http://yos.yj202588.top

echo "${s:0:5}"
来源：http://min.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://wlb.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbl.jyoumei.cn

[R24] 大小写转换
来源：http://jct.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eud.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://fsr.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tbi.tianlin.xyz

[R26] 命令替换
来源：http://ued.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://fwe.sufxvd.cn

[R27] 算术展开
来源：http://tog.iojbl.cn

echo $((1 + 2 * 3))
来源：http://heh.sweek.top

[R28] 浮点运算
来源：http://svv.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://xsf.epnwcf.com

[R29] 定义函数
来源：http://vgp.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsj.tianlin.xyz

[R30] 函数返回状态码
来源：http://vyd.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://pvq.hesvh.cn

[R31] 局部变量
来源：http://lyc.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://cqr.xinyue.icu

[R32] 参数个数校验
来源：http://opt.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://egm.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://iuy.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kaz.aibaodan.cn

[R34] 退出时清理
来源：http://gco.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://rrw.316326.xyz

[R35] 后台执行并等待
来源：http://oye.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zwh.jqgfzy.top

[R36] 并发执行多个任务
来源：http://owu.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oni.xylfe.cn

[R37] 把输出赋给变量
来源：http://upk.zhijiandao.cn

files=$(ls -1)
来源：http://mzh.daria6918.cn

[R38] 管道串联
来源：http://ows.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://coz.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://jej.hywenlv.cn

cmd > out.log 2>&1
来源：http://kyd.snrcjt.cn

[R40] 追加写日志
来源：http://znw.guowangkeji.top

echo "log" >> out.log
来源：http://szf.zycfv.cn

[R41] 丢弃输出
来源：http://oee.jianghu66.top

cmd >/dev/null 2>&1
来源：http://xka.yanxiufei.cn

[R42] 输入重定向
来源：http://ikv.vqdsnc.cn

wc -l < a.txt
来源：http://vkn.xziqi.cn

[R43] 按名字查找文件
来源：http://tns.xziqi.cn

find . -name "*.log" -type f
来源：http://mmg.meibo888.top

[R44] 按修改时间查找
来源：http://bdb.tanke756.top

find . -mtime -7 -type f
来源：http://zjf.xuanzx.com

[R45] 批量删除
来源：http://ifu.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://nrr.hammf.cn

[R46] 递归替换文件内容
来源：http://ekd.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pmi.hongshengwenyu.top

[R47] sed 单行替换
来源：http://ibr.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jja.xuanzx.com

[R48] awk 取指定列
来源：http://alx.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://inr.fengsongda.top

[R49] awk 带条件
来源：http://xdz.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dwd.shanyushiyangtech.top

[R50] awk 求和
来源：http://chc.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hfu.gaohongyu789.top

[R51] 排序去重取前几
来源：http://okl.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tvq.zhongyouzk.top

[R52] 统计行数
来源：http://ske.9152youxi.cn

wc -l a.txt
来源：http://plt.uphjek.com

[R53] 查看文件头与实时尾
来源：http://adv.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kmf.ydzc1.top

[R54] 比较两个文件
来源：http://vzv.hesvh.cn

diff a.txt b.txt
来源：http://don.bbcook.cn

[R55] 压缩与解压
来源：http://hvi.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rdz.birdmap.top

[R56] 远程拷贝
来源：http://mta.birdmap.top

scp file user@host:/path/
来源：http://goy.316326.xyz

[R57] 远程执行命令
来源：http://zdz.jqgufenzy.top

ssh user@host 'uptime'
来源：http://bhy.yonumen.top

[R58] 下载文件
来源：http://env.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://imj.shzxlz.cn

[R59] 发 POST JSON
来源：http://skh.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oea.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://fnz.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://otg.bjfxy.top

[R61] 磁盘占用
来源：http://avl.shuidangran.top

df -h;  du -sh *
来源：http://qfs.tian-w.cn

[R62] 找最占空间的文件
来源：http://eru.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://bjo.quarkkingdee.top

[R63] 内存与进程
来源：http://zxy.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://jgq.sxryk.cn

[R64] 结束进程
来源：http://hpl.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://oks.meibo888.top

[R65] 查看端口占用
来源：http://icx.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vzm.zhaomingkeji.xyz

[R66] 定时任务
来源：http://kaj.yuanzhike.top

crontab -e;  crontab -l
来源：http://gxn.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://fbf.yonumen.top

openssl rand -hex 16
来源：http://xfs.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://wrn.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://uec.tanke756.top

[R69] 生成随机密码
来源：http://hed.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://ehz.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://zaw.bjfxy.top

date +%s;  date -d @1700000000
来源：http://jor.redwolf501.top

[R71] 日期格式化
来源：http://ymg.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ouc.jqgfzy.top

[R72] 等待端口就绪
来源：http://iym.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kdp.yvedp.cn

[R73] 分割大日志
来源：http://gwa.guannengcc.top

split -l 1000 big.log part_
来源：http://gwh.xuetiantiany.cn

[R74] 批量重命名
来源：http://byb.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iew.9152youxi.cn

[R75] 导出环境变量
来源：http://qrb.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://dha.yanxiufei.cn

[R76] 使用临时文件
来源：http://xst.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qao.cheryme.top

[R77] 读取用户输入
来源：http://vyh.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://gln.yvedp.cn

[R78] 交互式菜单
来源：http://iit.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wmg.gzhubu.top

[R79] 解析命令行选项
来源：http://dwf.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wwo.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://nen.yfazqb.com

time ./run.sh
来源：http://zrw.pycfn.com

================================================================================
来源：http://agf.epnwcf.com


<!-- 参考信息 -->