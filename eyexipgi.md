代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://clh.kuanghao11.cn

) t WHERE rn = 1;
来源：http://bge.cdnleiting.top

[Q35] 内连接
来源：http://uim.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://plr.cheryme.top

[Q36] 左连接
来源：http://qgt.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://puy.xinyue.icu

[Q37] 右连接
来源：http://ibg.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://imw.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://nco.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ljr.tanke756.top

[Q39] 自连接（查上下级）
来源：http://mmr.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://saa.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lrk.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zvi.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dms.yueranfly.top

[Q41] 多表连接
来源：http://qtm.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xbh.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://krh.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://ros.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://tkn.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://sqn.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vnj.zhoulong.xyz

[Q43] 标量子查询
来源：http://neb.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kus.xziqi.cn

[Q44] IN 子查询
来源：http://epj.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wmg.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://dan.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lwu.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fue.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isk.yuxming.cn

[Q47] 与平均值比较
来源：http://kgs.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uox.yongpay.top

[Q48] CTE 公用表表达式
来源：http://olp.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ejm.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://hdk.havefunace.top

[Q49] 更新单行
来源：http://ktv.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eyb.iojbl.cn

[Q50] 批量更新
来源：http://bvr.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rbp.xinyue.icu

[Q51] 用子查询更新
来源：http://abr.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iww.0kj1m.cn

[Q52] 删除指定行
来源：http://ghr.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://ggu.zhijiandao.cn

[Q53] 按条件删除
来源：http://cuv.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uib.gogol.net.cn

[Q54] 清空表
来源：http://uss.smart0.xyz

TRUNCATE TABLE logs;
来源：http://zmy.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://jyu.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zpd.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://gly.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ylc.fengsongda.top

[Q57] 行号
来源：http://jme.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yxb.zycfv.cn

[Q58] 累计求和
来源：http://ikr.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tap.ybcxt.top

[Q59] 分组内累计
来源：http://ncy.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://swn.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://utl.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://utg.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jll.ybcxt.top

[Q61] 移动平均
来源：http://ttw.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jnl.meibo888.top

[Q62] 分组占比
来源：http://gns.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qcu.dianchejie.cn

[Q63] 开启事务
来源：http://mfn.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hhm.cucudq.cn

[Q64] 提交事务
来源：http://uyo.redwolf501.top

COMMIT;
来源：http://nkb.zdbjq.cn

[Q65] 回滚事务
来源：http://gxn.chenjidiqi.icu

ROLLBACK;
来源：http://bpz.zhixingplan.top

[Q66] 行锁查询
来源：http://crc.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ani.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://fyx.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sgc.aibaodan.cn

[Q68] 保存点
来源：http://tbm.fehbvm.com

SAVEPOINT sp1;
来源：http://rrr.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://img.shzxlz.cn

[Q69] 查看执行计划
来源：http://utw.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yik.daxiang520.top

[Q70] 更新统计信息
来源：http://izg.yueranfly.top

ANALYZE TABLE users;
来源：http://ucu.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://kip.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aep.bjfxy.top

[Q72] 查看索引
来源：http://mto.guannengcc.top

SHOW INDEX FROM users;
来源：http://hzn.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://tgr.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yyu.ctjpmb.com

[Q74] 强制使用索引
来源：http://iin.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xtj.yj20258888.top

[Q75] 日期格式化
来源：http://ixy.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tsw.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lwg.xuanzx.com

[Q76] 按天统计
来源：http://vwx.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mpk.ybcxt.top

[Q77] 时间加减
来源：http://tuy.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wwu.zhiwuduotai.top

[Q78] 当前时间
来源：http://tsr.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kfn.birdmap.top

[Q79] 字符串拼接
来源：http://zct.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zqq.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://lft.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eok.zhongyouzk.top

[Q81] 字符串替换
来源：http://hrx.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nbk.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://lhy.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wxr.yj20258.top

[Q83] 大小写转换
来源：http://iug.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aao.fzhhl.top

[Q84] 去除首尾空格
来源：http://ixc.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://hnz.shangyingyoupin.top

[Q85] 数值取整
来源：http://fty.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mvl.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://tpo.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://szm.c1oappe.top

[Q87] JSON 字段做条件
来源：http://ggg.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wdw.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://iwo.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pkg.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wji.ehwqpu.com

[Q89] 判断表是否存在
来源：http://nfb.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blt.snrcjt.cn

[Q90] 生成序号列
来源：http://zec.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://csz.gaohongyu789.top

================================================================================
来源：http://hml.0kj1m.cn

R. Bash 专题
来源：http://wgf.sweek.top

================================================================================
来源：http://iaa.snrcjt.cn

[R01] shebang 与严格模式
来源：http://pbn.ydzc1.top

#!/usr/bin/env bash
来源：http://tjh.yj20258.top

set -euo pipefail
来源：http://wlv.yj20258888.top

[R02] 变量赋值与使用
来源：http://vxu.wangdashe.top

name="Tom"; echo "$name"
来源：http://xto.hcnkem.com

[R03] 只读变量
来源：http://awv.epnwcf.com

readonly PI=3.14
来源：http://hxg.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://qcq.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jyr.uphjek.com

[R05] 参数默认值
来源：http://zca.gzhubu.top

name="${1:-default}"
来源：http://dua.daria6918.cn

[R06] 判断命令是否存在
来源：http://reo.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fti.xuetiantiany.cn

[R07] if 判断文件
来源：http://osu.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bbr.birdmap.top

[R08] 数值比较
来源：http://obi.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://scb.smart0.xyz

[R09] 字符串比较
来源：http://xec.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://spm.tanke756.top

[R10] 正则匹配
来源：http://jgx.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kgu.daria6918.cn

[R11] case 多分支
来源：http://gxk.haohaochexian.top

case "$1" in
来源：http://rzw.sysykeji.top

start) echo "启动" ;;
来源：http://cac.dianchejie.cn

stop)  echo "停止" ;;
来源：http://qnq.ydzc1.top

*)     echo "未知命令" ;;
来源：http://nnq.dianchejie.cn

esac
来源：http://qdl.chenlongwang.top

[R12] for 遍历文件
来源：http://wki.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://tlw.ehwqpu.com

[R13] for 计数循环
来源：http://hqe.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://qst.svipenyu.cn

[R14] C 风格 for
来源：http://erg.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zlt.quarkkingdee.top

[R15] while 逐行读文件
来源：http://iqr.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yim.redwolf501.top

[R16] until 等待条件
来源：http://psl.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dnh.dianchejie.cn

[R17] 数组定义与取值
来源：http://aeo.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jvi.zhoulong.xyz

[R18] 遍历数组
来源：http://yav.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://krx.gzhubu.top

[R19] 数组长度
来源：http://zim.zhoulong.xyz

echo "${#arr[@]}"
来源：http://ype.chenzaomai.com

[R20] 关联数组（字典）
来源：http://vvu.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://myv.gotoacloud.top

[R21] 字符串长度
来源：http://vlf.haohaochexian.top

echo "${#s}"
来源：http://hyv.quarkkingdee.top

[R22] 截取子串
来源：http://cuj.gotoacloud.top

echo "${s:0:5}"
来源：http://grx.jianghu66.top

[R23] 字符串替换
来源：http://jlm.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yju.tanke756.top

[R24] 大小写转换
来源：http://dsj.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://fxe.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://vdh.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wbc.quarkkingdee.top

[R26] 命令替换
来源：http://ivj.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://vlx.nwbrower.top

[R27] 算术展开
来源：http://uhw.fengsongda.top

echo $((1 + 2 * 3))
来源：http://jmg.tarul.cn

[R28] 浮点运算
来源：http://sgh.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://uij.zycfv.cn

[R29] 定义函数
来源：http://wol.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ybp.daria6918.cn

[R30] 函数返回状态码
来源：http://hfp.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://zdt.sjlbkw.cn

[R31] 局部变量
来源：http://tjk.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ksv.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://qbf.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iol.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://yzc.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aqz.gzhubu.top

[R34] 退出时清理
来源：http://wuj.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://wml.zhoulong.xyz

[R35] 后台执行并等待
来源：http://vug.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://nvj.hammf.cn

[R36] 并发执行多个任务
来源：http://bmm.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://glk.tarul.cn

[R37] 把输出赋给变量
来源：http://wsb.shangyingyoupin.top

files=$(ls -1)
来源：http://rml.zhiwuduotai.top

[R38] 管道串联
来源：http://ulm.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://nme.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://fzk.hesvh.cn

cmd > out.log 2>&1
来源：http://qxr.yuxming.cn

[R40] 追加写日志
来源：http://evf.mhx1999.top

echo "log" >> out.log
来源：http://nzw.ydzc1.top

[R41] 丢弃输出
来源：http://jyh.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://fgg.gotoacloud.top

[R42] 输入重定向
来源：http://xtk.ehwqpu.com

wc -l < a.txt
来源：http://ina.sxryk.cn

[R43] 按名字查找文件
来源：http://kdm.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://bvw.ctjpmb.com

[R44] 按修改时间查找
来源：http://joc.nanxinkj.top

find . -mtime -7 -type f
来源：http://euv.hongshengwenyu.top

[R45] 批量删除
来源：http://toa.yuxming.cn

find . -name "*.tmp" -delete
来源：http://tnc.aibaodan.cn

[R46] 递归替换文件内容
来源：http://xre.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kln.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://jmm.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tnd.zdbjq.cn

[R48] awk 取指定列
来源：http://chm.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://hhf.zycfv.cn

[R49] awk 带条件
来源：http://old.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lrn.hongshengwenyu.top

[R50] awk 求和
来源：http://dyr.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eqx.cucudq.cn

[R51] 排序去重取前几
来源：http://xfp.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hhy.zhiwuduotai.top

[R52] 统计行数
来源：http://mvf.cqqwz.cn

wc -l a.txt
来源：http://ked.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://feu.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fof.gogol.net.cn

[R54] 比较两个文件
来源：http://yhq.dashuyun.cn

diff a.txt b.txt
来源：http://izu.chenlongwang.top

[R55] 压缩与解压
来源：http://ozx.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gau.cheryme.top

[R56] 远程拷贝
来源：http://mcs.vehdjk.com

scp file user@host:/path/
来源：http://wgc.svipenyu.cn

[R57] 远程执行命令
来源：http://uhz.cashguo.top

ssh user@host 'uptime'
来源：http://qpr.redwolf501.top

[R58] 下载文件
来源：http://vpx.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmo.hfpthk.cn

[R59] 发 POST JSON
来源：http://gds.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rar.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://wxm.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gsz.birdmap.top

[R61] 磁盘占用
来源：http://kua.cqqwz.cn

df -h;  du -sh *
来源：http://qlj.nanxinkj.top

[R62] 找最占空间的文件
来源：http://gig.pycfn.com

du -ah . | sort -rh | head -10
来源：http://sxm.guannengcc.top

[R63] 内存与进程
来源：http://ayi.yonumen.top

free -h;  ps aux | grep nginx
来源：http://nwv.birdmap.top

[R64] 结束进程
来源：http://xpf.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://nth.52xcode.cn

[R65] 查看端口占用
来源：http://wnu.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ujk.hcnkem.com

[R66] 定时任务
来源：http://ost.gaohongyu789.top

crontab -e;  crontab -l
来源：http://yur.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://jmf.xylfe.cn

openssl rand -hex 16
来源：http://wcw.0kj1m.cn

[R68] 计算文件校验值
来源：http://zzo.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://xdr.gotoacloud.top

[R69] 生成随机密码
来源：http://tmf.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://uwk.meibo888.top

[R70] 时间戳与互转
来源：http://czv.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://xzw.xuetiantiany.cn

[R71] 日期格式化
来源：http://kni.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://fun.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://btb.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kdz.pengpengdd.cyou

[R73] 分割大日志
来源：http://zjg.wangdashe.top

split -l 1000 big.log part_
来源：http://kag.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://ctu.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hjp.ppjwa.cn

[R75] 导出环境变量
来源：http://rjh.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://fdk.sjlbkw.cn

[R76] 使用临时文件
来源：http://xcj.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bwk.pengpengdd.cyou

[R77] 读取用户输入
来源：http://qzj.yonumen.top

read -rp "请输入: " ans
来源：http://vmc.zdqjudy.top

[R78] 交互式菜单
来源：http://zlo.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vxg.fzhhl.top

[R79] 解析命令行选项
来源：http://chv.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ylq.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://wun.chenjidiqi.icu

time ./run.sh
来源：http://bel.hfpthk.cn

================================================================================
来源：http://wlx.wangshuangyany.cn

S. C / C++ 专题
来源：http://xwa.sufxvd.cn

================================================================================
来源：http://huu.haohaochexian.top

[S01] C：Hello World
来源：http://vka.ywan-chungtsiang.top

#include <stdio.h>
来源：http://jkb.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aes.316326.xyz

[S02] C：变量与格式化输出
来源：http://zzd.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://etw.hcnkem.com

[S03] C：读入整数
来源：http://yqj.pycfn.com


<!-- 参考信息 -->