代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://rom.dianchejie.cn

[Q30] 分组统计
来源：http://nzd.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rlt.zdqjudy.top

[Q31] 分组后过滤
来源：http://mcw.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lon.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://pyj.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cyl.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ytt.wangshuangyany.cn

[Q33] 多列分组
来源：http://cxh.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bnx.0kj1m.cn

[Q34] 每组取第一条
来源：http://elq.hammf.cn

SELECT * FROM (
来源：http://fuc.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://btl.chenzaomai.com

) t WHERE rn = 1;
来源：http://wln.fanxiaobao.xyz

[Q35] 内连接
来源：http://pzz.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lyx.yanxiufei.cn

[Q36] 左连接
来源：http://tue.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jvc.gaohongyu789.top

[Q37] 右连接
来源：http://tfj.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pjh.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://hjq.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vaa.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://jog.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yeo.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nar.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kcm.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ahc.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://pht.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://wpe.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://rgv.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://qyn.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://rlx.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://szp.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vlw.aibaodan.cn

[Q43] 标量子查询
来源：http://dmm.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://alu.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://sau.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://akb.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://yps.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oru.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jnm.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yer.mhx1999.top

[Q47] 与平均值比较
来源：http://fww.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://drp.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://vto.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ocr.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://ajy.wangdashe.top

[Q49] 更新单行
来源：http://ura.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yoz.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://kmn.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pih.yuanzhike.top

[Q51] 用子查询更新
来源：http://vyq.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://plc.andypj.xyz

[Q52] 删除指定行
来源：http://bzb.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://dwt.jqgfzy.top

[Q53] 按条件删除
来源：http://jiz.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qpz.yuanzhike.top

[Q54] 清空表
来源：http://sey.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://fph.cucudq.cn

[Q55] 排名（并列占位）
来源：http://goh.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://edm.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://uhp.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ask.jqgfzy.top

[Q57] 行号
来源：http://jln.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://syx.hcnkem.com

[Q58] 累计求和
来源：http://ddd.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dtr.yuanzhike.top

[Q59] 分组内累计
来源：http://nak.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dvx.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://drd.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://osm.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xai.316326.xyz

[Q61] 移动平均
来源：http://djd.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xam.epnwcf.com

[Q62] 分组占比
来源：http://woi.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xgk.jyoumei.cn

[Q63] 开启事务
来源：http://tjz.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://syr.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://nvb.gotoacloud.top

COMMIT;
来源：http://zic.sufxvd.cn

[Q65] 回滚事务
来源：http://gmy.ydzc1.top

ROLLBACK;
来源：http://kpt.hnxiangtu.top

[Q66] 行锁查询
来源：http://oic.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yzt.yvedp.cn

[Q67] 设置隔离级别
来源：http://tvg.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vlh.hywenlv.cn

[Q68] 保存点
来源：http://ldz.xylfe.cn

SAVEPOINT sp1;
来源：http://lgj.xuanzx.com

ROLLBACK TO sp1;
来源：http://ati.jinqigufen.top

[Q69] 查看执行计划
来源：http://fil.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://usk.gotoacloud.top

[Q70] 更新统计信息
来源：http://fxy.zhijiandao.cn

ANALYZE TABLE users;
来源：http://jdr.fengsongda.top

[Q71] 查看建表语句
来源：http://spp.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yvh.havefunace.top

[Q72] 查看索引
来源：http://sgz.guowangkeji.top

SHOW INDEX FROM users;
来源：http://xyu.316326.xyz

[Q73] 查看表状态
来源：http://dck.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uoi.yj20258888.top

[Q74] 强制使用索引
来源：http://nvy.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zio.bbcook.cn

[Q75] 日期格式化
来源：http://zgh.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ura.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pfb.xziqi.cn

[Q76] 按天统计
来源：http://yhh.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rpe.wangdashe.top

[Q77] 时间加减
来源：http://fzu.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jab.hcnkem.com

[Q78] 当前时间
来源：http://xde.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bbc.xinyue.icu

[Q79] 字符串拼接
来源：http://qar.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hjb.c1oappe.top

[Q80] 字符串截取
来源：http://xgn.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtm.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://emq.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ckf.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://iyc.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bfs.smart0.xyz

[Q83] 大小写转换
来源：http://jyj.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bwy.zdbjq.cn

[Q84] 去除首尾空格
来源：http://mek.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://mep.hywenlv.cn

[Q85] 数值取整
来源：http://hrt.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ffc.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://icb.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ari.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://fuv.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nyv.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://itn.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://myw.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hne.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://vnz.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bxv.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://ltu.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://feo.smart0.xyz

================================================================================
来源：http://ore.birdmap.top

R. Bash 专题
来源：http://ctg.xingfuxueyuan.xyz

================================================================================
来源：http://mwa.ppjwa.cn

[R01] shebang 与严格模式
来源：http://brj.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://atp.jqgufenzy.top

set -euo pipefail
来源：http://kid.dianchejie.cn

[R02] 变量赋值与使用
来源：http://zug.jianghu66.top

name="Tom"; echo "$name"
来源：http://edg.hcnkem.com

[R03] 只读变量
来源：http://yhf.cheryme.top

readonly PI=3.14
来源：http://kgq.0kj1m.cn

[R04] 位置参数
来源：http://urw.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jki.sweek.top

[R05] 参数默认值
来源：http://hup.aibaodan.cn

name="${1:-default}"
来源：http://lwk.xuanzx.com

[R06] 判断命令是否存在
来源：http://rra.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dyu.hfpthk.cn

[R07] if 判断文件
来源：http://plp.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xyo.wangshuangyany.cn

[R08] 数值比较
来源：http://dag.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eyn.fktsv.cn

[R09] 字符串比较
来源：http://hhf.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrv.316326.xyz

[R10] 正则匹配
来源：http://nvt.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dec.fktsv.cn

[R11] case 多分支
来源：http://wzp.yuxming.cn

case "$1" in
来源：http://apl.fehbvm.com

start) echo "启动" ;;
来源：http://uvv.yfazqb.com

stop)  echo "停止" ;;
来源：http://auf.nwbrower.top

*)     echo "未知命令" ;;
来源：http://bcm.zdqjudy.top

esac
来源：http://tzc.52xcode.cn

[R12] for 遍历文件
来源：http://zbt.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://bdk.xuanzx.com

[R13] for 计数循环
来源：http://llj.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://bee.gaohongyu789.top

[R14] C 风格 for
来源：http://rlz.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uef.ppjwa.cn

[R15] while 逐行读文件
来源：http://zdr.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://moj.shanyushiyangtech.top

[R16] until 等待条件
来源：http://rdf.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hmx.hysaishi.cn

[R17] 数组定义与取值
来源：http://lxj.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://yla.uphjek.com

[R18] 遍历数组
来源：http://ulu.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vph.mhx1999.top

[R19] 数组长度
来源：http://eju.hnqzz.top

echo "${#arr[@]}"
来源：http://bby.cucudq.cn

[R20] 关联数组（字典）
来源：http://mxd.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kiz.hnxiangtu.top

[R21] 字符串长度
来源：http://kfl.svipenyu.cn

echo "${#s}"
来源：http://dxw.pycfn.com

[R22] 截取子串
来源：http://okk.zhixingplan.top

echo "${s:0:5}"
来源：http://zrh.meibo888.top

[R23] 字符串替换
来源：http://tjc.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bjx.jqgufenzy.top

[R24] 大小写转换
来源：http://xls.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kei.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://gsq.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://svh.jinqigufen.top

[R26] 命令替换
来源：http://nbg.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://uph.wangdashe.top

[R27] 算术展开
来源：http://utj.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://ich.hnxiangtu.top

[R28] 浮点运算
来源：http://nws.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://cae.shuidangran.top

[R29] 定义函数
来源：http://jzn.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jmo.yuanzhike.top

[R30] 函数返回状态码
来源：http://jki.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://vci.sjlbkw.cn

[R31] 局部变量
来源：http://cob.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://njk.smart0.xyz

[R32] 参数个数校验
来源：http://umz.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gpn.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://gul.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyn.chenzaomai.com

[R34] 退出时清理
来源：http://pol.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://shg.birdmap.top

[R35] 后台执行并等待
来源：http://nuz.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://mov.shuidangran.top

[R36] 并发执行多个任务
来源：http://ulx.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://awt.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://dbd.sysykeji.top

files=$(ls -1)
来源：http://che.ehwqpu.com

[R38] 管道串联
来源：http://umr.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://umf.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://ocz.ybcxt.top

cmd > out.log 2>&1
来源：http://yrp.zycfv.cn

[R40] 追加写日志
来源：http://vqu.snrcjt.cn

echo "log" >> out.log
来源：http://nqw.yanxiufei.cn

[R41] 丢弃输出
来源：http://vqw.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://kgb.pycfn.com

[R42] 输入重定向
来源：http://dot.shuidangran.top

wc -l < a.txt
来源：http://jqx.meibo888.top

[R43] 按名字查找文件
来源：http://vlf.ydzc1.top

find . -name "*.log" -type f
来源：http://mbc.xylfe.cn

[R44] 按修改时间查找
来源：http://qds.yongpay.top

find . -mtime -7 -type f
来源：http://fgo.sufxvd.cn

[R45] 批量删除
来源：http://qvt.ivvv.top

find . -name "*.tmp" -delete
来源：http://hfd.chenzaomai.com

[R46] 递归替换文件内容
来源：http://mvh.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xgh.iojbl.cn

[R47] sed 单行替换
来源：http://lsh.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rou.jiagoushi.top

[R48] awk 取指定列
来源：http://vsw.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://vyr.daria6918.cn

[R49] awk 带条件
来源：http://ngv.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://okj.yfazqb.com

[R50] awk 求和
来源：http://gdo.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://cbp.kuanghao11.cn

[R51] 排序去重取前几
来源：http://pai.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fwr.hfpthk.cn

[R52] 统计行数
来源：http://kix.hywenlv.cn

wc -l a.txt
来源：http://vtd.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://rbq.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xfj.ybcxt.top

[R54] 比较两个文件
来源：http://sim.cqqwz.cn

diff a.txt b.txt
来源：http://spo.yanxiufei.cn

[R55] 压缩与解压
来源：http://ihi.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jif.cheryme.top

[R56] 远程拷贝
来源：http://wxm.aizwys.cn

scp file user@host:/path/
来源：http://nfc.quarkkingdee.top

[R57] 远程执行命令
来源：http://ovq.cucudq.cn

ssh user@host 'uptime'
来源：http://eke.chenzaomai.com

[R58] 下载文件
来源：http://wxg.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bxw.zhongyouzk.top

[R59] 发 POST JSON
来源：http://kno.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yrz.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://zcu.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jqt.wangshuangyany.cn

[R61] 磁盘占用
来源：http://wdd.nanxinkj.top

df -h;  du -sh *
来源：http://hmu.sxryk.cn

[R62] 找最占空间的文件
来源：http://llf.sufxvd.cn

du -ah . | sort -rh | head -10
来源：http://sdj.havefunace.top

[R63] 内存与进程
来源：http://ryp.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://lci.fanxiaobao.xyz

[R64] 结束进程
来源：http://rlk.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://cvi.guowangkeji.top

[R65] 查看端口占用
来源：http://tsa.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dal.zhiwuduotai.top

[R66] 定时任务
来源：http://tyo.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://msi.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://tcn.xuanzx.com

openssl rand -hex 16
来源：http://ppq.ybcxt.top

[R68] 计算文件校验值
来源：http://pik.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xyt.nwbrower.top

[R69] 生成随机密码
来源：http://iat.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://nfm.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://xnb.xinyue.icu

date +%s;  date -d @1700000000
来源：http://bpm.vqdsnc.cn

[R71] 日期格式化
来源：http://fjh.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nuf.yj20258.top

[R72] 等待端口就绪
来源：http://ndf.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ktg.wangshuangyany.cn

[R73] 分割大日志
来源：http://zqy.jinqigufen.top

split -l 1000 big.log part_
来源：http://chf.xinyue.icu

[R74] 批量重命名
来源：http://vyz.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kam.ppjwa.cn

[R75] 导出环境变量
来源：http://cyo.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://wmf.svipenyu.cn

[R76] 使用临时文件
来源：http://vcb.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dzv.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://gqo.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://clh.hnxiangtu.top

[R78] 交互式菜单
来源：http://fag.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xmw.wangdashe.top

[R79] 解析命令行选项
来源：http://yhf.mhx1999.top


<!-- 参考信息 -->