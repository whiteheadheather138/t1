代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfz.guannengcc.top

[Q32] 分组拼接字符串
来源：http://pvv.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eit.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://trj.yangfankeji.com

[Q33] 多列分组
来源：http://xkc.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kna.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://grq.fanxiaobao.xyz

SELECT * FROM (
来源：http://kzm.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ski.daxiang520.top

) t WHERE rn = 1;
来源：http://wcm.fktsv.cn

[Q35] 内连接
来源：http://yxe.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://czi.shuidangran.top

[Q36] 左连接
来源：http://zbw.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://llz.havefunace.top

[Q37] 右连接
来源：http://ygj.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://paf.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://log.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tlw.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://iqh.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrs.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lhh.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://soy.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bji.aizwys.cn

[Q41] 多表连接
来源：http://pda.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://edc.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://sqd.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://wal.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://qyw.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://ubt.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://scd.yanxiufei.cn

[Q43] 标量子查询
来源：http://sxo.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://net.havefunace.top

[Q44] IN 子查询
来源：http://hme.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vpw.uphjek.com

[Q45] EXISTS 判断存在
来源：http://guv.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hdp.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://nsk.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yyw.smart0.xyz

[Q47] 与平均值比较
来源：http://mlc.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ick.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://alf.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kfg.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://nip.hnqzz.top

[Q49] 更新单行
来源：http://qhf.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yyq.xziqi.cn

[Q50] 批量更新
来源：http://uik.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wjh.meibo888.top

[Q51] 用子查询更新
来源：http://hvz.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qgh.tarul.cn

[Q52] 删除指定行
来源：http://geb.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://zkc.hesvh.cn

[Q53] 按条件删除
来源：http://nca.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kaf.ctjpmb.com

[Q54] 清空表
来源：http://jza.yj20258888.top

TRUNCATE TABLE logs;
来源：http://fld.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://qty.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rfa.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://ojk.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yli.snrcjt.cn

[Q57] 行号
来源：http://pkw.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pgr.havefunace.top

[Q58] 累计求和
来源：http://llu.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gra.tanke756.top

[Q59] 分组内累计
来源：http://adl.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zsb.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://zoq.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lwi.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jpj.dashuyun.cn

[Q61] 移动平均
来源：http://sab.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nha.zhengqikj.top

[Q62] 分组占比
来源：http://tsm.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ixc.cashguo.top

[Q63] 开启事务
来源：http://hdd.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ona.shuidangran.top

[Q64] 提交事务
来源：http://xqr.jinqigfzy.top

COMMIT;
来源：http://cgs.yonumen.top

[Q65] 回滚事务
来源：http://bgr.hcnkem.com

ROLLBACK;
来源：http://met.yfazqb.com

[Q66] 行锁查询
来源：http://gaq.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tvv.havefunace.top

[Q67] 设置隔离级别
来源：http://uwu.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gdu.ctjpmb.com

[Q68] 保存点
来源：http://tcj.9152youxi.cn

SAVEPOINT sp1;
来源：http://ysr.redwolf501.top

ROLLBACK TO sp1;
来源：http://quq.zhongyouzk.top

[Q69] 查看执行计划
来源：http://tuc.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sao.wangdashe.top

[Q70] 更新统计信息
来源：http://gfq.sjlbkw.cn

ANALYZE TABLE users;
来源：http://aob.yonumen.top

[Q71] 查看建表语句
来源：http://gik.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cde.jiagoushi.top

[Q72] 查看索引
来源：http://qmh.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://dvo.jqgfzy.top

[Q73] 查看表状态
来源：http://mnq.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ilm.zhongyouzk.top

[Q74] 强制使用索引
来源：http://vth.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jqi.yanxiufei.cn

[Q75] 日期格式化
来源：http://ryu.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yaj.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yie.yj20258.top

[Q76] 按天统计
来源：http://ldy.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pcm.hongshengwenyu.top

[Q77] 时间加减
来源：http://slc.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgc.yangfankeji.com

[Q78] 当前时间
来源：http://vqn.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rdi.ydjk.org.cn

[Q79] 字符串拼接
来源：http://wcm.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uvh.dianchejie.cn

[Q80] 字符串截取
来源：http://yvr.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hzw.gaohongyu789.top

[Q81] 字符串替换
来源：http://nfk.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tel.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://olh.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://grn.vqdsnc.cn

[Q83] 大小写转换
来源：http://vxd.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://erf.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://slb.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://apj.guannengcc.top

[Q85] 数值取整
来源：http://lue.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dla.tanke756.top

[Q86] 读取 JSON 字段
来源：http://cjp.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pco.tian-w.cn

[Q87] JSON 字段做条件
来源：http://eeq.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nbo.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://rof.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kgb.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://usg.nwbrower.top

[Q89] 判断表是否存在
来源：http://mdo.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dlh.cashguo.top

[Q90] 生成序号列
来源：http://bdj.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pfj.jyoumei.cn

================================================================================
来源：http://wbo.guowangkeji.top

R. Bash 专题
来源：http://lze.zhiwuduotai.top

================================================================================
来源：http://byy.gogol.net.cn

[R01] shebang 与严格模式
来源：http://xve.yj20258.top

#!/usr/bin/env bash
来源：http://egh.hfpthk.cn

set -euo pipefail
来源：http://kfe.guowangkeji.top

[R02] 变量赋值与使用
来源：http://zxl.guannengcc.top

name="Tom"; echo "$name"
来源：http://uke.hammf.cn

[R03] 只读变量
来源：http://qbv.zhiwuduotai.top

readonly PI=3.14
来源：http://ybs.fktsv.cn

[R04] 位置参数
来源：http://qnk.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cay.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://rqq.ywan-chungtsiang.top

name="${1:-default}"
来源：http://why.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://zny.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eod.ydjk.org.cn

[R07] if 判断文件
来源：http://xnl.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tpf.xuetiantiany.cn

[R08] 数值比较
来源：http://sjj.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ggw.xziqi.cn

[R09] 字符串比较
来源：http://qmz.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yus.daxiang520.top

[R10] 正则匹配
来源：http://cbp.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dlz.xylfe.cn

[R11] case 多分支
来源：http://foe.zhongyouzk.top

case "$1" in
来源：http://ctu.wangdashe.top

start) echo "启动" ;;
来源：http://mzb.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://aes.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://hla.yanxiufei.cn

esac
来源：http://fvo.birdmap.top

[R12] for 遍历文件
来源：http://wrg.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://hjk.fzhhl.top

[R13] for 计数循环
来源：http://rvb.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://izq.yfazqb.com

[R14] C 风格 for
来源：http://uud.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mdu.yj20258.top

[R15] while 逐行读文件
来源：http://arl.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mnh.svipenyu.cn

[R16] until 等待条件
来源：http://oss.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zks.birdmap.top

[R17] 数组定义与取值
来源：http://vpp.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://wfg.chenjidiqi.icu

[R18] 遍历数组
来源：http://rjf.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://njf.jinqigfzy.top

[R19] 数组长度
来源：http://pfl.aibaodan.cn

echo "${#arr[@]}"
来源：http://qju.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://vdj.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://joz.vehdjk.com

[R21] 字符串长度
来源：http://myw.ybcxt.top

echo "${#s}"
来源：http://kqz.yvedp.cn

[R22] 截取子串
来源：http://cpg.guowangkeji.top

echo "${s:0:5}"
来源：http://xbg.chenjidiqi.icu

[R23] 字符串替换
来源：http://ivn.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wyt.jinqigufen.top

[R24] 大小写转换
来源：http://xjt.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://xgc.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://kke.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ted.ybcxt.top

[R26] 命令替换
来源：http://jfo.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://eki.cdnleiting.top

[R27] 算术展开
来源：http://tnp.yonumen.top

echo $((1 + 2 * 3))
来源：http://zur.dashuyun.cn

[R28] 浮点运算
来源：http://ocf.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://gnx.ydjk.org.cn

[R29] 定义函数
来源：http://kyn.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://umy.daxiang520.top

[R30] 函数返回状态码
来源：http://swo.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://fld.hcnkem.com

[R31] 局部变量
来源：http://yel.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://kxs.hnxiangtu.top

[R32] 参数个数校验
来源：http://sdf.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxt.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://qjp.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ttq.zycfv.cn

[R34] 退出时清理
来源：http://ici.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ozy.dianchejie.cn

[R35] 后台执行并等待
来源：http://lwh.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mck.xuanzx.com

[R36] 并发执行多个任务
来源：http://sno.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ely.iojbl.cn

[R37] 把输出赋给变量
来源：http://byu.pengpengdd.cyou

files=$(ls -1)
来源：http://pov.sufxvd.cn

[R38] 管道串联
来源：http://ffy.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://mtr.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://qjo.tian-w.cn

cmd > out.log 2>&1
来源：http://abz.cucudq.cn

[R40] 追加写日志
来源：http://vcb.hcnkem.com

echo "log" >> out.log
来源：http://lzt.hesvh.cn

[R41] 丢弃输出
来源：http://ckv.guannengcc.top

cmd >/dev/null 2>&1
来源：http://dla.zhixingplan.top

[R42] 输入重定向
来源：http://kuo.andypj.xyz

wc -l < a.txt
来源：http://dlr.fzhhl.top

[R43] 按名字查找文件
来源：http://jcr.zhoulong.xyz

find . -name "*.log" -type f
来源：http://jhx.daria6918.cn

[R44] 按修改时间查找
来源：http://pcg.bbcook.cn

find . -mtime -7 -type f
来源：http://ipc.316326.xyz

[R45] 批量删除
来源：http://xpe.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://rgf.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://woj.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uft.wangdashe.top

[R47] sed 单行替换
来源：http://fbd.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://acq.havefunace.top

[R48] awk 取指定列
来源：http://vgq.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://qgx.zhongyouzk.top

[R49] awk 带条件
来源：http://qhb.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xed.xinyue.icu

[R50] awk 求和
来源：http://etr.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://ouk.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://hnv.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zvt.snrcjt.cn

[R52] 统计行数
来源：http://qyg.ivvv.top

wc -l a.txt
来源：http://ilr.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://tdo.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgf.aizwys.cn

[R54] 比较两个文件
来源：http://wzm.vehdjk.com

diff a.txt b.txt
来源：http://ukl.jinqigfzy.top

[R55] 压缩与解压
来源：http://fhc.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pfp.ivvv.top

[R56] 远程拷贝
来源：http://wzw.zhongyouzk.top

scp file user@host:/path/
来源：http://dlq.yfazqb.com

[R57] 远程执行命令
来源：http://zws.yanxiufei.cn

ssh user@host 'uptime'
来源：http://lfy.xuanzx.com

[R58] 下载文件
来源：http://jvv.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vnv.hfpthk.cn

[R59] 发 POST JSON
来源：http://icu.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oxw.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://onw.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://naz.dashuyun.cn

[R61] 磁盘占用
来源：http://yqp.svipenyu.cn

df -h;  du -sh *
来源：http://dgi.fzhhl.top

[R62] 找最占空间的文件
来源：http://bdj.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://sba.316326.xyz

[R63] 内存与进程
来源：http://xte.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://bdz.wangshuangyany.cn

[R64] 结束进程
来源：http://qaq.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://awy.fehbvm.com

[R65] 查看端口占用
来源：http://vbn.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ymk.shangyingyoupin.top

[R66] 定时任务
来源：http://tkf.yongpay.top

crontab -e;  crontab -l
来源：http://gck.yonumen.top

[R67] 生成随机十六进制串
来源：http://glf.zdbjq.cn

openssl rand -hex 16
来源：http://psx.mhx1999.top

[R68] 计算文件校验值
来源：http://qzv.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://fsl.kuanghao11.cn

[R69] 生成随机密码
来源：http://oyl.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://dga.tianlin.xyz

[R70] 时间戳与互转
来源：http://hup.aizwys.cn

date +%s;  date -d @1700000000
来源：http://jbr.guowangkeji.top

[R71] 日期格式化
来源：http://thw.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sho.ydjk.org.cn

[R72] 等待端口就绪
来源：http://onw.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ism.zdbjq.cn

[R73] 分割大日志
来源：http://ani.hcnkem.com

split -l 1000 big.log part_
来源：http://sqr.52xcode.cn

[R74] 批量重命名
来源：http://kyk.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://klz.chenlongwang.top

[R75] 导出环境变量
来源：http://teu.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://psy.sufxvd.cn

[R76] 使用临时文件
来源：http://xso.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lhe.yj20258.top

[R77] 读取用户输入
来源：http://ecp.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://udb.yuxming.cn

[R78] 交互式菜单
来源：http://kfq.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://alr.hywenlv.cn

[R79] 解析命令行选项
来源：http://jnf.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ytt.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://pqp.fzhhl.top

time ./run.sh
来源：http://izv.fengsongda.top

================================================================================
来源：http://ngz.wangshuangyany.cn


<!-- 参考信息 -->