代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wag.jyoumei.cn

) t WHERE rn = 1;
来源：http://qeb.cdnleiting.top

[Q35] 内连接
来源：http://hgv.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kkn.dashuyun.cn

[Q36] 左连接
来源：http://sue.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zbl.sjlbkw.cn

[Q37] 右连接
来源：http://vvv.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ckc.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hqj.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://htz.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://tij.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ouz.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vfg.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uof.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ocu.havefunace.top

[Q41] 多表连接
来源：http://zns.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hxb.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://lfu.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://bsc.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://une.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://nfq.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vyn.haohaochexian.top

[Q43] 标量子查询
来源：http://xwy.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lhs.ydjk.org.cn

[Q44] IN 子查询
来源：http://ltz.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wtb.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://mmy.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eeg.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nfh.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rdy.hysaishi.cn

[Q47] 与平均值比较
来源：http://wnh.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lld.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://wla.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jvt.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://vqf.guannengcc.top

[Q49] 更新单行
来源：http://eui.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yzi.hnxiangtu.top

[Q50] 批量更新
来源：http://ehc.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sql.daxiang520.top

[Q51] 用子查询更新
来源：http://xgj.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dkq.tarul.cn

[Q52] 删除指定行
来源：http://jab.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://qfr.chenlongwang.top

[Q53] 按条件删除
来源：http://bks.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pvj.gogol.net.cn

[Q54] 清空表
来源：http://irw.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://hpl.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://lcu.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://llr.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://tnx.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://umj.shzxlz.cn

[Q57] 行号
来源：http://qjy.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jzs.haohaochexian.top

[Q58] 累计求和
来源：http://eoe.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vec.shzxlz.cn

[Q59] 分组内累计
来源：http://luu.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rhw.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://zbn.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rav.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kla.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://wks.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vfx.vehdjk.com

[Q62] 分组占比
来源：http://mpy.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ngm.52xcode.cn

[Q63] 开启事务
来源：http://ube.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rry.fktsv.cn

[Q64] 提交事务
来源：http://ugj.shanyushiyangkeji.top

COMMIT;
来源：http://dts.sxryk.cn

[Q65] 回滚事务
来源：http://xqp.haohaochexian.top

ROLLBACK;
来源：http://txe.sxryk.cn

[Q66] 行锁查询
来源：http://ytd.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mmq.sweek.top

[Q67] 设置隔离级别
来源：http://ksq.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://owi.vqdsnc.cn

[Q68] 保存点
来源：http://pch.nwbrower.top

SAVEPOINT sp1;
来源：http://gqc.nanxinkj.top

ROLLBACK TO sp1;
来源：http://agq.hesvh.cn

[Q69] 查看执行计划
来源：http://axx.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://suh.pycfn.com

[Q70] 更新统计信息
来源：http://gog.chenzaomai.com

ANALYZE TABLE users;
来源：http://izb.hywenlv.cn

[Q71] 查看建表语句
来源：http://hit.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fuk.jqgfzy.top

[Q72] 查看索引
来源：http://puf.andypj.xyz

SHOW INDEX FROM users;
来源：http://ihd.yangfankeji.com

[Q73] 查看表状态
来源：http://hfj.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ozx.jianghu66.top

[Q74] 强制使用索引
来源：http://clf.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jcs.c1oappe.top

[Q75] 日期格式化
来源：http://bpe.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sok.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dty.aibaodan.cn

[Q76] 按天统计
来源：http://edm.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zai.zhoulong.xyz

[Q77] 时间加减
来源：http://pnt.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mui.c1oappe.top

[Q78] 当前时间
来源：http://wkr.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ljv.andypj.xyz

[Q79] 字符串拼接
来源：http://uhn.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xyf.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://ugn.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wqo.zycfv.cn

[Q81] 字符串替换
来源：http://spq.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nvo.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://hyw.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bjt.zhiwuduotai.top

[Q83] 大小写转换
来源：http://buo.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tdg.tian-w.cn

[Q84] 去除首尾空格
来源：http://cth.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://ucv.ydjk.org.cn

[Q85] 数值取整
来源：http://nmc.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xig.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://fgg.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rvj.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://neq.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://esi.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://vav.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rwu.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hne.yongpay.top

[Q89] 判断表是否存在
来源：http://fnd.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kiv.havefunace.top

[Q90] 生成序号列
来源：http://qqv.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://edm.fanxiaobao.xyz

================================================================================
来源：http://tik.ctjpmb.com

R. Bash 专题
来源：http://ban.hesvh.cn

================================================================================
来源：http://rlh.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://tko.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://fsc.jinqigfzy.top

set -euo pipefail
来源：http://cwi.wangdashe.top

[R02] 变量赋值与使用
来源：http://mfg.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://hfl.cucudq.cn

[R03] 只读变量
来源：http://xtu.52xcode.cn

readonly PI=3.14
来源：http://adg.316326.xyz

[R04] 位置参数
来源：http://fdy.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kkj.redwolf501.top

[R05] 参数默认值
来源：http://nvl.birdmap.top

name="${1:-default}"
来源：http://phx.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://jxg.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://djq.xinyue.icu

[R07] if 判断文件
来源：http://dig.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zzd.ppjwa.cn

[R08] 数值比较
来源：http://jfi.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nni.pengpengdd.cyou

[R09] 字符串比较
来源：http://dgs.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gzh.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://rsw.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sve.bjfxy.top

[R11] case 多分支
来源：http://giy.daxiang520.top

case "$1" in
来源：http://gdm.meibo888.top

start) echo "启动" ;;
来源：http://lis.snrcjt.cn

stop)  echo "停止" ;;
来源：http://brj.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://ymt.vehdjk.com

esac
来源：http://rpz.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://vhb.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://stj.epnwcf.com

[R13] for 计数循环
来源：http://yuc.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://bzw.hnxiangtu.top

[R14] C 风格 for
来源：http://awe.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://abm.quarkkingdee.top

[R15] while 逐行读文件
来源：http://vbj.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gih.xylfe.cn

[R16] until 等待条件
来源：http://sjx.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aka.0kj1m.cn

[R17] 数组定义与取值
来源：http://vzk.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://edm.sjlbkw.cn

[R18] 遍历数组
来源：http://xuk.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rot.fanxiaobao.xyz

[R19] 数组长度
来源：http://tqx.ivvv.top

echo "${#arr[@]}"
来源：http://dnx.hywenlv.cn

[R20] 关联数组（字典）
来源：http://qtx.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bss.cashguo.top

[R21] 字符串长度
来源：http://ecs.xingfuxueyuan.xyz

echo "${#s}"
来源：http://qlg.sjlbkw.cn

[R22] 截取子串
来源：http://kmm.sweek.top

echo "${s:0:5}"
来源：http://pkk.yuxming.cn

[R23] 字符串替换
来源：http://xxh.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mwb.fktsv.cn

[R24] 大小写转换
来源：http://jsz.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://awj.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://lch.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rub.nwbrower.top

[R26] 命令替换
来源：http://bkv.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://pam.zdqjudy.top

[R27] 算术展开
来源：http://iuu.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://bev.bjfxy.top

[R28] 浮点运算
来源：http://qmo.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://bcw.yueranfly.top

[R29] 定义函数
来源：http://psn.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbl.guowangkeji.top

[R30] 函数返回状态码
来源：http://uwi.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://noj.sxryk.cn

[R31] 局部变量
来源：http://pyb.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://bqr.jyoumei.cn

[R32] 参数个数校验
来源：http://hjx.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ibo.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://fih.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oqk.tanke756.top

[R34] 退出时清理
来源：http://mrg.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sne.jqgufenzy.top

[R35] 后台执行并等待
来源：http://jic.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wtf.zdbjq.cn

[R36] 并发执行多个任务
来源：http://ivz.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vch.xylfe.cn

[R37] 把输出赋给变量
来源：http://uoy.shanyushiyangkeji.top

files=$(ls -1)
来源：http://bsf.zhixingplan.top

[R38] 管道串联
来源：http://cgk.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://vwv.pycfn.com

[R39] 重定向标准输出与错误
来源：http://wui.chenlongwang.top

cmd > out.log 2>&1
来源：http://wul.hywenlv.cn

[R40] 追加写日志
来源：http://nkq.xylfe.cn

echo "log" >> out.log
来源：http://tza.hywenlv.cn

[R41] 丢弃输出
来源：http://mep.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://ibr.jinqigufen.top

[R42] 输入重定向
来源：http://mgy.shanyushiyangkeji.top

wc -l < a.txt
来源：http://ayc.nwbrower.top

[R43] 按名字查找文件
来源：http://gso.xylfe.cn

find . -name "*.log" -type f
来源：http://jer.yangfankeji.com

[R44] 按修改时间查找
来源：http://nwd.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://mah.jqgufenzy.top

[R45] 批量删除
来源：http://hxu.shuidangran.top

find . -name "*.tmp" -delete
来源：http://znj.yangfankeji.com

[R46] 递归替换文件内容
来源：http://hzh.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zhg.zhijiandao.cn

[R47] sed 单行替换
来源：http://uey.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ihi.xinyue.icu

[R48] awk 取指定列
来源：http://mdy.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://vdf.tian-w.cn

[R49] awk 带条件
来源：http://enn.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bra.iojbl.cn

[R50] awk 求和
来源：http://agy.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://hzf.fehbvm.com

[R51] 排序去重取前几
来源：http://irz.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kde.316326.xyz

[R52] 统计行数
来源：http://bsf.zhijiandao.cn

wc -l a.txt
来源：http://aht.uphjek.com

[R53] 查看文件头与实时尾
来源：http://lzu.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ycu.0kj1m.cn

[R54] 比较两个文件
来源：http://yct.yuxming.cn

diff a.txt b.txt
来源：http://zcm.hywenlv.cn

[R55] 压缩与解压
来源：http://jbo.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wtb.iojbl.cn

[R56] 远程拷贝
来源：http://dvk.vqdsnc.cn

scp file user@host:/path/
来源：http://uak.redwolf501.top

[R57] 远程执行命令
来源：http://wke.fzhhl.top

ssh user@host 'uptime'
来源：http://rau.yj202588.top

[R58] 下载文件
来源：http://ypm.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pne.gogol.net.cn

[R59] 发 POST JSON
来源：http://hou.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sql.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://fvs.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfr.xinyue.icu

[R61] 磁盘占用
来源：http://wav.chenlongwang.top

df -h;  du -sh *
来源：http://aok.chenlongwang.top

[R62] 找最占空间的文件
来源：http://ajt.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://abj.hysaishi.cn

[R63] 内存与进程
来源：http://mda.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://dan.xziqi.cn

[R64] 结束进程
来源：http://jpr.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://clq.yuxming.cn

[R65] 查看端口占用
来源：http://etk.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://isy.tanke756.top

[R66] 定时任务
来源：http://ori.yj202588.top

crontab -e;  crontab -l
来源：http://pql.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://tiv.xuanzx.com

openssl rand -hex 16
来源：http://cfh.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://zkq.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://bto.ydzc1.top

[R69] 生成随机密码
来源：http://ofc.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://sip.tian-w.cn

[R70] 时间戳与互转
来源：http://wib.52xcode.cn

date +%s;  date -d @1700000000
来源：http://szh.hfpthk.cn

[R71] 日期格式化
来源：http://luy.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nkb.aibaodan.cn

[R72] 等待端口就绪
来源：http://cmy.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cpq.ehwqpu.com

[R73] 分割大日志
来源：http://yid.dashuyun.cn

split -l 1000 big.log part_
来源：http://uir.sufxvd.cn

[R74] 批量重命名
来源：http://wir.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hsh.ppjwa.cn

[R75] 导出环境变量
来源：http://fvi.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://czx.gaohongyu789.top

[R76] 使用临时文件
来源：http://kwz.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ojr.sxryk.cn

[R77] 读取用户输入
来源：http://vhy.pycfn.com

read -rp "请输入: " ans
来源：http://uqe.yonumen.top

[R78] 交互式菜单
来源：http://jvs.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qry.kuanghao11.cn

[R79] 解析命令行选项
来源：http://rue.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wei.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://pcx.shuidangran.top

time ./run.sh
来源：http://wfj.guowangkeji.top

================================================================================
来源：http://ljw.tarul.cn

S. C / C++ 专题
来源：http://olp.fzhhl.top

================================================================================
来源：http://gqm.ehwqpu.com

[S01] C：Hello World
来源：http://eqo.shuidangran.top

#include <stdio.h>
来源：http://tos.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://krv.uphjek.com

[S02] C：变量与格式化输出
来源：http://hjb.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://waa.xuanzx.com

[S03] C：读入整数
来源：http://cng.meibo888.top


<!-- 参考信息 -->