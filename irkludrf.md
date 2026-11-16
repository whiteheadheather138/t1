代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dju.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://fac.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pis.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aqu.fktsv.cn

[Q33] 多列分组
来源：http://gto.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://joh.bjfxy.top

[Q34] 每组取第一条
来源：http://tvg.ivvv.top

SELECT * FROM (
来源：http://vnk.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oew.ydzc1.top

) t WHERE rn = 1;
来源：http://dcs.daxiang520.top

[Q35] 内连接
来源：http://kng.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jis.tianlin.xyz

[Q36] 左连接
来源：http://gyw.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ycx.zhengqikj.top

[Q37] 右连接
来源：http://vaa.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ijp.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://kee.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tkd.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://vdh.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bfy.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vrw.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uqs.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jlg.ivvv.top

[Q41] 多表连接
来源：http://iek.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jhk.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://chq.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://jqi.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://cve.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://hel.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pgg.yueranfly.top

[Q43] 标量子查询
来源：http://zns.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imb.zdqjudy.top

[Q44] IN 子查询
来源：http://cvr.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wrv.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://sok.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ltv.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://tgr.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ulq.yangfankeji.com

[Q47] 与平均值比较
来源：http://hvr.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://umd.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://ptw.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://twf.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://hqn.birdmap.top

[Q49] 更新单行
来源：http://hpl.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://clz.xylfe.cn

[Q50] 批量更新
来源：http://wjg.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ohh.xuanzx.com

[Q51] 用子查询更新
来源：http://aoy.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fpb.nwbrower.top

[Q52] 删除指定行
来源：http://mmk.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://hbb.gotoacloud.top

[Q53] 按条件删除
来源：http://qce.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://asu.fanxiaobao.xyz

[Q54] 清空表
来源：http://wdw.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://euf.sweek.top

[Q55] 排名（并列占位）
来源：http://wby.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yjm.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://yxt.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lmt.xingfuxueyuan.xyz

[Q57] 行号
来源：http://gti.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dhw.jqgufenzy.top

[Q58] 累计求和
来源：http://bpr.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngn.hesvh.cn

[Q59] 分组内累计
来源：http://phl.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mmp.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://lvq.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blq.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://whw.zhengqikj.top

[Q61] 移动平均
来源：http://hhv.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ayx.hesvh.cn

[Q62] 分组占比
来源：http://fuc.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ipn.guowangkeji.top

[Q63] 开启事务
来源：http://rul.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nji.gaohongyu789.top

[Q64] 提交事务
来源：http://bvk.hysaishi.cn

COMMIT;
来源：http://aht.fehbvm.com

[Q65] 回滚事务
来源：http://ybb.shuidangran.top

ROLLBACK;
来源：http://sfx.yongpay.top

[Q66] 行锁查询
来源：http://mox.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ewq.fzhhl.top

[Q67] 设置隔离级别
来源：http://daf.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dcd.0kj1m.cn

[Q68] 保存点
来源：http://jkk.hammf.cn

SAVEPOINT sp1;
来源：http://hrm.daxiang520.top

ROLLBACK TO sp1;
来源：http://dta.9152youxi.cn

[Q69] 查看执行计划
来源：http://iga.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wxx.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://nzr.c1oappe.top

ANALYZE TABLE users;
来源：http://mva.aibaodan.cn

[Q71] 查看建表语句
来源：http://yqn.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://boi.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://imc.52xcode.cn

SHOW INDEX FROM users;
来源：http://vxb.yuxming.cn

[Q73] 查看表状态
来源：http://rxh.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://arq.meibo888.top

[Q74] 强制使用索引
来源：http://cjm.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gsn.wangdashe.top

[Q75] 日期格式化
来源：http://lzb.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://erh.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yki.tian-w.cn

[Q76] 按天统计
来源：http://dny.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fbt.yonumen.top

[Q77] 时间加减
来源：http://bos.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gvt.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://szz.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://myy.iojbl.cn

[Q79] 字符串拼接
来源：http://acy.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ata.xuetiantiany.cn

[Q80] 字符串截取
来源：http://hgl.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nsg.guowangkeji.top

[Q81] 字符串替换
来源：http://hkb.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nul.cashguo.top

[Q82] 字符长度与字节长度
来源：http://aoh.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fvn.dianchejie.cn

[Q83] 大小写转换
来源：http://eui.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sgn.dianchejie.cn

[Q84] 去除首尾空格
来源：http://bqv.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://rdp.jinqigufen.top

[Q85] 数值取整
来源：http://jlc.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bzs.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://qdq.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ovi.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://ani.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ypt.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://vak.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twm.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cvc.dianchejie.cn

[Q89] 判断表是否存在
来源：http://jwb.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uld.shangyingyoupin.top

[Q90] 生成序号列
来源：http://dla.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyz.jlsjyb.cn

================================================================================
来源：http://hoe.0kj1m.cn

R. Bash 专题
来源：http://iob.jiagoushi.top

================================================================================
来源：http://gfa.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://eij.bjfxy.top

#!/usr/bin/env bash
来源：http://jds.gogol.net.cn

set -euo pipefail
来源：http://viq.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://dxm.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://fhh.jqgfzy.top

[R03] 只读变量
来源：http://rjs.fehbvm.com

readonly PI=3.14
来源：http://vod.fktsv.cn

[R04] 位置参数
来源：http://gmh.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wzh.daxiang520.top

[R05] 参数默认值
来源：http://hhz.tanke756.top

name="${1:-default}"
来源：http://ixn.xziqi.cn

[R06] 判断命令是否存在
来源：http://wgs.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://agu.jqgfzy.top

[R07] if 判断文件
来源：http://wdo.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jnl.aibaodan.cn

[R08] 数值比较
来源：http://sbp.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://itq.feifeiyinyue.top

[R09] 字符串比较
来源：http://wch.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yfk.daria6918.cn

[R10] 正则匹配
来源：http://vsm.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hwf.cheryme.top

[R11] case 多分支
来源：http://xqf.xuetiantiany.cn

case "$1" in
来源：http://dup.dashuyun.cn

start) echo "启动" ;;
来源：http://tdq.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://xxd.c1oappe.top

*)     echo "未知命令" ;;
来源：http://mjm.shuidangran.top

esac
来源：http://kwf.jinqigufen.top

[R12] for 遍历文件
来源：http://kfz.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://bvn.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://mlz.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://jnq.shzxlz.cn

[R14] C 风格 for
来源：http://igu.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uag.zhixingplan.top

[R15] while 逐行读文件
来源：http://ier.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gls.ctjpmb.com

[R16] until 等待条件
来源：http://nfw.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zzw.yongpay.top

[R17] 数组定义与取值
来源：http://cpl.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://qss.jqgfzy.top

[R18] 遍历数组
来源：http://bgb.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://znp.meibo888.top

[R19] 数组长度
来源：http://wvo.epnwcf.com

echo "${#arr[@]}"
来源：http://dtb.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://odk.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iex.chenjidiqi.icu

[R21] 字符串长度
来源：http://pmd.snrcjt.cn

echo "${#s}"
来源：http://uvg.aibaodan.cn

[R22] 截取子串
来源：http://dcx.chenzaomai.com

echo "${s:0:5}"
来源：http://bnm.fengsongda.top

[R23] 字符串替换
来源：http://kfd.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hmc.cqqwz.cn

[R24] 大小写转换
来源：http://cjo.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qek.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://oah.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gln.guannengcc.top

[R26] 命令替换
来源：http://qmf.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://thh.quarkkingdee.top

[R27] 算术展开
来源：http://ddq.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://bjj.xuetiantiany.cn

[R28] 浮点运算
来源：http://bcs.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://usv.feifeiyinyue.top

[R29] 定义函数
来源：http://eeh.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kgp.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://nec.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://uhk.jyoumei.cn

[R31] 局部变量
来源：http://cmi.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://wgs.andypj.xyz

[R32] 参数个数校验
来源：http://zly.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyh.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://bgx.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nyu.zhixingplan.top

[R34] 退出时清理
来源：http://ldm.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://kbu.9152youxi.cn

[R35] 后台执行并等待
来源：http://clo.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zws.gzhubu.top

[R36] 并发执行多个任务
来源：http://zse.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://six.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://ixl.wangshuangyany.cn

files=$(ls -1)
来源：http://izi.0kj1m.cn

[R38] 管道串联
来源：http://wmp.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://txd.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://ubw.daxiang520.top

cmd > out.log 2>&1
来源：http://ixn.ppjwa.cn

[R40] 追加写日志
来源：http://dkk.yangfankeji.com

echo "log" >> out.log
来源：http://inw.ivvv.top

[R41] 丢弃输出
来源：http://zwc.cashguo.top

cmd >/dev/null 2>&1
来源：http://ale.aibaodan.cn

[R42] 输入重定向
来源：http://bdf.zhengqikj.top

wc -l < a.txt
来源：http://hqo.bjfxy.top

[R43] 按名字查找文件
来源：http://zqm.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://wkk.9152youxi.cn

[R44] 按修改时间查找
来源：http://lmj.yfazqb.com

find . -mtime -7 -type f
来源：http://mhj.fktsv.cn

[R45] 批量删除
来源：http://qnw.ivvv.top

find . -name "*.tmp" -delete
来源：http://pps.jyoumei.cn

[R46] 递归替换文件内容
来源：http://rpv.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://epk.ctjpmb.com

[R47] sed 单行替换
来源：http://pku.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gzs.meibo888.top

[R48] awk 取指定列
来源：http://vbt.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://rsp.jqgufenzy.top

[R49] awk 带条件
来源：http://jdr.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ppk.tianlin.xyz

[R50] awk 求和
来源：http://fbm.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hok.tianlin.xyz

[R51] 排序去重取前几
来源：http://ccr.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eqb.cqqwz.cn

[R52] 统计行数
来源：http://fzt.uphjek.com

wc -l a.txt
来源：http://cub.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://erp.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kdy.chenzaomai.com

[R54] 比较两个文件
来源：http://vqb.ydzc1.top

diff a.txt b.txt
来源：http://fjx.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://iwk.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nlu.hnqzz.top

[R56] 远程拷贝
来源：http://uuf.xuanzx.com

scp file user@host:/path/
来源：http://lia.nwbrower.top

[R57] 远程执行命令
来源：http://ivt.gzhubu.top

ssh user@host 'uptime'
来源：http://sho.shanyushiyangtech.top

[R58] 下载文件
来源：http://bmv.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dem.jqgfzy.top

[R59] 发 POST JSON
来源：http://dii.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yyf.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://skh.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zjw.dashuyun.cn

[R61] 磁盘占用
来源：http://ars.svipenyu.cn

df -h;  du -sh *
来源：http://qya.yuanzhike.top

[R62] 找最占空间的文件
来源：http://eqw.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://lbw.yonumen.top

[R63] 内存与进程
来源：http://mio.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://zii.guowangkeji.top

[R64] 结束进程
来源：http://eyl.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://fbx.tianlin.xyz

[R65] 查看端口占用
来源：http://lav.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fvx.daria6918.cn

[R66] 定时任务
来源：http://zku.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://eyt.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://lgg.cashguo.top

openssl rand -hex 16
来源：http://pqc.sjlbkw.cn

[R68] 计算文件校验值
来源：http://ayq.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oxk.pycfn.com

[R69] 生成随机密码
来源：http://ldn.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://pri.yvedp.cn

[R70] 时间戳与互转
来源：http://xmt.yj20258.top

date +%s;  date -d @1700000000
来源：http://aks.svipenyu.cn

[R71] 日期格式化
来源：http://xae.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qdq.yj202588.top

[R72] 等待端口就绪
来源：http://mfa.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oxd.yueranfly.top

[R73] 分割大日志
来源：http://irq.kuanghao11.cn

split -l 1000 big.log part_
来源：http://ljj.0kj1m.cn

[R74] 批量重命名
来源：http://cac.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://idz.hammf.cn

[R75] 导出环境变量
来源：http://zcv.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://dbu.tian-w.cn

[R76] 使用临时文件
来源：http://mot.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ccl.shzxlz.cn

[R77] 读取用户输入
来源：http://lnw.cucudq.cn

read -rp "请输入: " ans
来源：http://tfg.zycfv.cn

[R78] 交互式菜单
来源：http://vco.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://npj.zhijiandao.cn

[R79] 解析命令行选项
来源：http://ggi.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ssf.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://vvj.hcnkem.com

time ./run.sh
来源：http://gsm.hesvh.cn

================================================================================
来源：http://adq.bjfxy.top


<!-- 参考信息 -->