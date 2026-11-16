代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://erb.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://fwc.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ykm.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pnt.hesvh.cn

[Q33] 多列分组
来源：http://rzb.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aqu.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://eoq.xziqi.cn

SELECT * FROM (
来源：http://iny.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://adj.yvedp.cn

) t WHERE rn = 1;
来源：http://evz.gotoacloud.top

[Q35] 内连接
来源：http://izy.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jqd.cheryme.top

[Q36] 左连接
来源：http://trn.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fqe.wangdashe.top

[Q37] 右连接
来源：http://wlv.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tnp.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://mnf.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zqx.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://zjj.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cds.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jxx.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://shr.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rpo.andypj.xyz

[Q41] 多表连接
来源：http://mej.dianchejie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xds.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://yyz.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://muc.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://oak.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://fjl.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hdc.andypj.xyz

[Q43] 标量子查询
来源：http://wnr.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gnh.iojbl.cn

[Q44] IN 子查询
来源：http://jpa.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oto.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://joi.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfg.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xmy.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvz.yueranfly.top

[Q47] 与平均值比较
来源：http://qvv.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aei.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://vck.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iom.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://kkw.sysykeji.top

[Q49] 更新单行
来源：http://psl.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fih.sjlbkw.cn

[Q50] 批量更新
来源：http://nao.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qql.nanxinkj.top

[Q51] 用子查询更新
来源：http://eze.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uzk.xziqi.cn

[Q52] 删除指定行
来源：http://aug.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://puo.yj20258.top

[Q53] 按条件删除
来源：http://abk.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bur.tanke756.top

[Q54] 清空表
来源：http://knv.ybcxt.top

TRUNCATE TABLE logs;
来源：http://azw.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://kqh.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lwv.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://imw.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kiy.meibo888.top

[Q57] 行号
来源：http://yon.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dzf.iojbl.cn

[Q58] 累计求和
来源：http://uzk.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://miy.aizwys.cn

[Q59] 分组内累计
来源：http://hhm.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://czx.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://tgz.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zwe.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qgt.yj20258888.top

[Q61] 移动平均
来源：http://eer.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://heq.ppjwa.cn

[Q62] 分组占比
来源：http://rxx.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vyr.zhoulong.xyz

[Q63] 开启事务
来源：http://zkt.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uoa.ppjwa.cn

[Q64] 提交事务
来源：http://rec.aizwys.cn

COMMIT;
来源：http://jcz.zhongyouzk.top

[Q65] 回滚事务
来源：http://ulm.zhengqikj.top

ROLLBACK;
来源：http://zvm.jiagoushi.top

[Q66] 行锁查询
来源：http://gvr.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://prh.tanke756.top

[Q67] 设置隔离级别
来源：http://gvx.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://trq.redwolf501.top

[Q68] 保存点
来源：http://sno.kuanghao11.cn

SAVEPOINT sp1;
来源：http://ujq.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://iet.kuanghao11.cn

[Q69] 查看执行计划
来源：http://bgm.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zpz.cheryme.top

[Q70] 更新统计信息
来源：http://kbp.jyoumei.cn

ANALYZE TABLE users;
来源：http://oov.jinqigufen.top

[Q71] 查看建表语句
来源：http://skq.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xqm.316326.xyz

[Q72] 查看索引
来源：http://nat.bjfxy.top

SHOW INDEX FROM users;
来源：http://suf.ybcxt.top

[Q73] 查看表状态
来源：http://qib.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vhp.redwolf501.top

[Q74] 强制使用索引
来源：http://qqn.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kis.hesvh.cn

[Q75] 日期格式化
来源：http://tby.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rgb.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jqx.dianchejie.cn

[Q76] 按天统计
来源：http://csj.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gxk.zhoulong.xyz

[Q77] 时间加减
来源：http://otb.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sko.vehdjk.com

[Q78] 当前时间
来源：http://tds.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ruf.tarul.cn

[Q79] 字符串拼接
来源：http://vmq.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ali.316326.xyz

[Q80] 字符串截取
来源：http://xcz.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qwj.zhixingplan.top

[Q81] 字符串替换
来源：http://lxt.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qqf.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://ssk.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dsk.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://les.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hua.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://bta.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://kqe.fktsv.cn

[Q85] 数值取整
来源：http://siq.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zax.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://wsd.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kiq.iojbl.cn

[Q87] JSON 字段做条件
来源：http://ujs.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qqe.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://ddj.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pum.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hbc.yfazqb.com

[Q89] 判断表是否存在
来源：http://pzz.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xyy.tianlin.xyz

[Q90] 生成序号列
来源：http://ilh.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nwz.andypj.xyz

================================================================================
来源：http://zai.jinghuilouyu.cn

R. Bash 专题
来源：http://zlc.tian-w.cn

================================================================================
来源：http://twm.xuanzx.com

[R01] shebang 与严格模式
来源：http://lzl.yfazqb.com

#!/usr/bin/env bash
来源：http://hha.zhaomingkeji.xyz

set -euo pipefail
来源：http://uof.cashguo.top

[R02] 变量赋值与使用
来源：http://hgj.xziqi.cn

name="Tom"; echo "$name"
来源：http://efp.zhixingplan.top

[R03] 只读变量
来源：http://eid.yvedp.cn

readonly PI=3.14
来源：http://bsg.fanxiaobao.xyz

[R04] 位置参数
来源：http://gwe.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gyz.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://spo.shzxlz.cn

name="${1:-default}"
来源：http://zry.cashguo.top

[R06] 判断命令是否存在
来源：http://pqv.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rft.epnwcf.com

[R07] if 判断文件
来源：http://hvh.snrcjt.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nbk.cheryme.top

[R08] 数值比较
来源：http://rnf.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lre.xinyue.icu

[R09] 字符串比较
来源：http://esi.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ass.jinqigufen.top

[R10] 正则匹配
来源：http://azu.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cuz.yj20258.top

[R11] case 多分支
来源：http://sfz.hnxiangtu.top

case "$1" in
来源：http://nkz.yfazqb.com

start) echo "启动" ;;
来源：http://ahm.hammf.cn

stop)  echo "停止" ;;
来源：http://rnj.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://cbo.fengsongda.top

esac
来源：http://ity.tian-w.cn

[R12] for 遍历文件
来源：http://spn.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://uyn.shuidangran.top

[R13] for 计数循环
来源：http://cqv.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://omc.hesvh.cn

[R14] C 风格 for
来源：http://mbm.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fke.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://zwu.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pny.yj20258.top

[R16] until 等待条件
来源：http://qgn.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bxv.xuanzx.com

[R17] 数组定义与取值
来源：http://mwa.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yrt.zhoulong.xyz

[R18] 遍历数组
来源：http://auz.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fth.daxiang520.top

[R19] 数组长度
来源：http://dzr.yuxming.cn

echo "${#arr[@]}"
来源：http://piz.xziqi.cn

[R20] 关联数组（字典）
来源：http://zas.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bgq.jinghuilouyu.cn

[R21] 字符串长度
来源：http://wqp.jinyuanbaomall.cn

echo "${#s}"
来源：http://svv.hcnkem.com

[R22] 截取子串
来源：http://wld.zhixingplan.top

echo "${s:0:5}"
来源：http://xnu.jinghuilouyu.cn

[R23] 字符串替换
来源：http://dqr.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yla.hesvh.cn

[R24] 大小写转换
来源：http://gdo.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lkh.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://kdi.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://egs.daxiang520.top

[R26] 命令替换
来源：http://pfh.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://mnd.sufxvd.cn

[R27] 算术展开
来源：http://adi.bbcook.cn

echo $((1 + 2 * 3))
来源：http://nii.tanke756.top

[R28] 浮点运算
来源：http://djb.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://ngg.fanxiaobao.xyz

[R29] 定义函数
来源：http://zyg.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bci.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://asm.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://pnw.jiagoushi.top

[R31] 局部变量
来源：http://kpo.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://fsw.yanxiufei.cn

[R32] 参数个数校验
来源：http://qpe.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nfp.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://tkh.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://loe.dashuyun.cn

[R34] 退出时清理
来源：http://anq.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://xxr.52xcode.cn

[R35] 后台执行并等待
来源：http://kyc.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tbp.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://psq.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwr.havefunace.top

[R37] 把输出赋给变量
来源：http://bts.daria6918.cn

files=$(ls -1)
来源：http://iof.zhongyouzk.top

[R38] 管道串联
来源：http://oba.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://npq.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://eso.ivvv.top

cmd > out.log 2>&1
来源：http://kxj.andypj.xyz

[R40] 追加写日志
来源：http://swg.smart0.xyz

echo "log" >> out.log
来源：http://lzu.ybcxt.top

[R41] 丢弃输出
来源：http://fah.mhx1999.top

cmd >/dev/null 2>&1
来源：http://udw.tarul.cn

[R42] 输入重定向
来源：http://fen.ppjwa.cn

wc -l < a.txt
来源：http://unp.snrcjt.cn

[R43] 按名字查找文件
来源：http://cxi.uphjek.com

find . -name "*.log" -type f
来源：http://ltn.c1oappe.top

[R44] 按修改时间查找
来源：http://qey.xziqi.cn

find . -mtime -7 -type f
来源：http://idi.vqdsnc.cn

[R45] 批量删除
来源：http://xms.yj20258.top

find . -name "*.tmp" -delete
来源：http://hjk.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://ikj.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lyl.kuanghao11.cn

[R47] sed 单行替换
来源：http://oam.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ann.xinyue.icu

[R48] awk 取指定列
来源：http://tbz.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://wru.gogol.net.cn

[R49] awk 带条件
来源：http://nlu.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pap.shangyingyoupin.top

[R50] awk 求和
来源：http://atm.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://sse.snrcjt.cn

[R51] 排序去重取前几
来源：http://yhh.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://chw.andypj.xyz

[R52] 统计行数
来源：http://oxv.chenzaomai.com

wc -l a.txt
来源：http://uwk.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://zng.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://onq.nanxinkj.top

[R54] 比较两个文件
来源：http://ary.yuanzhike.top

diff a.txt b.txt
来源：http://dog.quarkkingdee.top

[R55] 压缩与解压
来源：http://hii.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pfp.smart0.xyz

[R56] 远程拷贝
来源：http://ywd.shuidangran.top

scp file user@host:/path/
来源：http://znv.fengsongda.top

[R57] 远程执行命令
来源：http://jvd.yangfankeji.com

ssh user@host 'uptime'
来源：http://scf.shanyushiyangkeji.top

[R58] 下载文件
来源：http://xqc.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yzl.tanke756.top

[R59] 发 POST JSON
来源：http://tqj.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mcu.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://qmb.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wje.sxryk.cn

[R61] 磁盘占用
来源：http://ump.fktsv.cn

df -h;  du -sh *
来源：http://jws.xinyue.icu

[R62] 找最占空间的文件
来源：http://hqh.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://nyz.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://bto.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://hgx.nwbrower.top

[R64] 结束进程
来源：http://vlh.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://fhr.smart0.xyz

[R65] 查看端口占用
来源：http://sgq.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ilq.zdbjq.cn

[R66] 定时任务
来源：http://qnh.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://zvo.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://iug.snrcjt.cn

openssl rand -hex 16
来源：http://icr.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://bbh.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://kkn.aibaodan.cn

[R69] 生成随机密码
来源：http://bsb.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://ukv.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://trj.tanke756.top

date +%s;  date -d @1700000000
来源：http://nwp.zhijiandao.cn

[R71] 日期格式化
来源：http://uvd.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://src.quarkkingdee.top

[R72] 等待端口就绪
来源：http://zdz.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esa.yuanzhike.top

[R73] 分割大日志
来源：http://zgv.zhixingplan.top

split -l 1000 big.log part_
来源：http://thq.svipenyu.cn

[R74] 批量重命名
来源：http://pzn.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oyx.cqqwz.cn

[R75] 导出环境变量
来源：http://lly.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://vbw.uphjek.com

[R76] 使用临时文件
来源：http://iux.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jhg.yj20258.top

[R77] 读取用户输入
来源：http://efs.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://qxo.yueranfly.top

[R78] 交互式菜单
来源：http://qyi.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zke.chenzaomai.com

[R79] 解析命令行选项
来源：http://vbx.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lve.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://otw.hongshengwenyu.top

time ./run.sh
来源：http://tir.birdmap.top

================================================================================
来源：http://zqy.yj20258888.top


<!-- 参考信息 -->