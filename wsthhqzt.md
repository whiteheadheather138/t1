代发 wailian999

[Q33] 多列分组
来源：http://hcx.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iem.zhengqikj.top

[Q34] 每组取第一条
来源：http://fwk.yfazqb.com

SELECT * FROM (
来源：http://cmn.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://osa.jqgufenzy.top

) t WHERE rn = 1;
来源：http://gkc.fengsongda.top

[Q35] 内连接
来源：http://vap.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yez.chenlongwang.top

[Q36] 左连接
来源：http://krw.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://erf.yj20258.top

[Q37] 右连接
来源：http://apy.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hsh.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vji.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ojf.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://eir.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cvq.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iur.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vfh.tianlin.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tyc.ctjpmb.com

[Q41] 多表连接
来源：http://dgu.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nxz.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://lpi.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://tmm.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://jgg.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://efw.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dme.zycfv.cn

[Q43] 标量子查询
来源：http://yom.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iqp.yvedp.cn

[Q44] IN 子查询
来源：http://lqn.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lxd.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://mph.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://meg.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://ljp.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wro.xziqi.cn

[Q47] 与平均值比较
来源：http://nfs.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lid.yj20258.top

[Q48] CTE 公用表表达式
来源：http://pmz.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://suj.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://aug.ivvv.top

[Q49] 更新单行
来源：http://szg.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dbo.hnqzz.top

[Q50] 批量更新
来源：http://yhd.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qgb.316326.xyz

[Q51] 用子查询更新
来源：http://xte.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hyd.cqqwz.cn

[Q52] 删除指定行
来源：http://gnh.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://vhw.zhongyouzk.top

[Q53] 按条件删除
来源：http://qzi.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tjw.yueranfly.top

[Q54] 清空表
来源：http://xgt.tian-w.cn

TRUNCATE TABLE logs;
来源：http://ygf.xziqi.cn

[Q55] 排名（并列占位）
来源：http://fwf.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hjn.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://qmk.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dhx.xinyue.icu

[Q57] 行号
来源：http://deq.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tzh.kuanghao11.cn

[Q58] 累计求和
来源：http://arx.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kys.yonumen.top

[Q59] 分组内累计
来源：http://lvp.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hik.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://uuq.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jne.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qkw.ivvv.top

[Q61] 移动平均
来源：http://lbh.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hzj.meibo888.top

[Q62] 分组占比
来源：http://efu.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bmp.jinqigfzy.top

[Q63] 开启事务
来源：http://ggg.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dhm.yuxming.cn

[Q64] 提交事务
来源：http://tsc.meibo888.top

COMMIT;
来源：http://dsf.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://efh.ydjk.org.cn

ROLLBACK;
来源：http://szo.xuanzx.com

[Q66] 行锁查询
来源：http://oyy.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xkb.dianchejie.cn

[Q67] 设置隔离级别
来源：http://hmp.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tcl.c1oappe.top

[Q68] 保存点
来源：http://pvd.nwbrower.top

SAVEPOINT sp1;
来源：http://ppe.jiagoushi.top

ROLLBACK TO sp1;
来源：http://vev.yuxming.cn

[Q69] 查看执行计划
来源：http://ziu.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zfd.fengsongda.top

[Q70] 更新统计信息
来源：http://zzw.shzxlz.cn

ANALYZE TABLE users;
来源：http://ecy.cdnleiting.top

[Q71] 查看建表语句
来源：http://kuw.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uoh.gotoacloud.top

[Q72] 查看索引
来源：http://gwi.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://spu.guowangkeji.top

[Q73] 查看表状态
来源：http://pcz.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fuz.zycfv.cn

[Q74] 强制使用索引
来源：http://grw.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://opx.sweek.top

[Q75] 日期格式化
来源：http://xzi.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jdu.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dmu.fehbvm.com

[Q76] 按天统计
来源：http://izs.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bbg.jiagoushi.top

[Q77] 时间加减
来源：http://lam.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tav.sysykeji.top

[Q78] 当前时间
来源：http://ebr.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wwx.cheryme.top

[Q79] 字符串拼接
来源：http://pyn.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rja.pycfn.com

[Q80] 字符串截取
来源：http://krh.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vrl.hongshengwenyu.top

[Q81] 字符串替换
来源：http://ifz.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hlf.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://pmm.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eww.316326.xyz

[Q83] 大小写转换
来源：http://ewn.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rae.yuanzhike.top

[Q84] 去除首尾空格
来源：http://jhe.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://yrx.ppjwa.cn

[Q85] 数值取整
来源：http://nfq.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nju.ivvv.top

[Q86] 读取 JSON 字段
来源：http://gbz.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gnc.daria6918.cn

[Q87] JSON 字段做条件
来源：http://lez.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nib.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://wpq.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uqw.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zfx.cdnleiting.top

[Q89] 判断表是否存在
来源：http://nrn.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://caj.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://ygt.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iwo.52xcode.cn

================================================================================
来源：http://crv.andypj.xyz

R. Bash 专题
来源：http://rxp.wangshuangyany.cn

================================================================================
来源：http://iij.mhx1999.top

[R01] shebang 与严格模式
来源：http://ulb.jqgfzy.top

#!/usr/bin/env bash
来源：http://tbb.fktsv.cn

set -euo pipefail
来源：http://ops.ctjpmb.com

[R02] 变量赋值与使用
来源：http://ohw.hnqzz.top

name="Tom"; echo "$name"
来源：http://xzh.shuidangran.top

[R03] 只读变量
来源：http://vuk.tanke756.top

readonly PI=3.14
来源：http://bmb.cheryme.top

[R04] 位置参数
来源：http://ogk.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lqu.iojbl.cn

[R05] 参数默认值
来源：http://ojw.0kj1m.cn

name="${1:-default}"
来源：http://xyd.xziqi.cn

[R06] 判断命令是否存在
来源：http://abv.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vat.shanyushiyangtech.top

[R07] if 判断文件
来源：http://fby.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fky.52xcode.cn

[R08] 数值比较
来源：http://lyv.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nhf.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://thv.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ode.zhengqikj.top

[R10] 正则匹配
来源：http://jam.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://smx.yuxming.cn

[R11] case 多分支
来源：http://vwc.hongshengwenyu.top

case "$1" in
来源：http://thk.shangyingyoupin.top

start) echo "启动" ;;
来源：http://wqe.yuxming.cn

stop)  echo "停止" ;;
来源：http://abx.zycfv.cn

*)     echo "未知命令" ;;
来源：http://ctf.yfazqb.com

esac
来源：http://xeb.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://fwl.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://fwt.yuanzhike.top

[R13] for 计数循环
来源：http://vtd.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://ivq.gzhubu.top

[R14] C 风格 for
来源：http://qfv.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://asy.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://swh.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mdp.aizwys.cn

[R16] until 等待条件
来源：http://rde.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cil.yj20258.top

[R17] 数组定义与取值
来源：http://dcc.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://ttz.jianghu66.top

[R18] 遍历数组
来源：http://cgs.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wol.nanxinkj.top

[R19] 数组长度
来源：http://mro.smart0.xyz

echo "${#arr[@]}"
来源：http://als.gotoacloud.top

[R20] 关联数组（字典）
来源：http://ybl.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://btm.shuidangran.top

[R21] 字符串长度
来源：http://iyc.cqqwz.cn

echo "${#s}"
来源：http://yyt.zhongyouzk.top

[R22] 截取子串
来源：http://fhy.sjlbkw.cn

echo "${s:0:5}"
来源：http://snf.mhx1999.top

[R23] 字符串替换
来源：http://xlm.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ylw.uphjek.com

[R24] 大小写转换
来源：http://ceh.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hpt.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://nje.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wyv.fengsongda.top

[R26] 命令替换
来源：http://hke.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://dun.dashuyun.cn

[R27] 算术展开
来源：http://wkc.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://pjq.xziqi.cn

[R28] 浮点运算
来源：http://qpo.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://boi.ppjwa.cn

[R29] 定义函数
来源：http://izc.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gyi.yueranfly.top

[R30] 函数返回状态码
来源：http://ooe.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://pwv.bbcook.cn

[R31] 局部变量
来源：http://sku.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://zzv.yueranfly.top

[R32] 参数个数校验
来源：http://otj.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nrn.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://pno.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gic.tarul.cn

[R34] 退出时清理
来源：http://yxv.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://urm.yj20258.top

[R35] 后台执行并等待
来源：http://tag.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qjy.guannengcc.top

[R36] 并发执行多个任务
来源：http://wjo.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ned.jiagoushi.top

[R37] 把输出赋给变量
来源：http://gpz.yj202588.top

files=$(ls -1)
来源：http://vrk.fzhhl.top

[R38] 管道串联
来源：http://fau.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://cyy.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://alp.yonumen.top

cmd > out.log 2>&1
来源：http://ptg.tarul.cn

[R40] 追加写日志
来源：http://bud.smart0.xyz

echo "log" >> out.log
来源：http://cqq.hongshengwenyu.top

[R41] 丢弃输出
来源：http://lpy.fktsv.cn

cmd >/dev/null 2>&1
来源：http://nvh.ehwqpu.com

[R42] 输入重定向
来源：http://vsf.yonumen.top

wc -l < a.txt
来源：http://mxq.yuanzhike.top

[R43] 按名字查找文件
来源：http://tmp.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://pxu.zdbjq.cn

[R44] 按修改时间查找
来源：http://qpk.sufxvd.cn

find . -mtime -7 -type f
来源：http://nvh.bjfxy.top

[R45] 批量删除
来源：http://wzv.xziqi.cn

find . -name "*.tmp" -delete
来源：http://sxq.jinqigufen.top

[R46] 递归替换文件内容
来源：http://nql.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hcg.0kj1m.cn

[R47] sed 单行替换
来源：http://gzx.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://tcp.cucudq.cn

[R48] awk 取指定列
来源：http://wxf.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://drf.yj20258.top

[R49] awk 带条件
来源：http://azh.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xvp.wangdashe.top

[R50] awk 求和
来源：http://aqr.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://dmq.jyoumei.cn

[R51] 排序去重取前几
来源：http://nao.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qhh.yj202588.top

[R52] 统计行数
来源：http://nwg.ydzc1.top

wc -l a.txt
来源：http://xxf.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://bdr.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fqd.wangdashe.top

[R54] 比较两个文件
来源：http://bzg.nwbrower.top

diff a.txt b.txt
来源：http://wbf.daria6918.cn

[R55] 压缩与解压
来源：http://xue.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jyo.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://afv.nanxinkj.top

scp file user@host:/path/
来源：http://wnu.feifeiyinyue.top

[R57] 远程执行命令
来源：http://wfe.9152youxi.cn

ssh user@host 'uptime'
来源：http://fgb.sjlbkw.cn

[R58] 下载文件
来源：http://xpc.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jlk.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://jgu.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jeg.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://njp.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://skn.sufxvd.cn

[R61] 磁盘占用
来源：http://ywq.yuanzhike.top

df -h;  du -sh *
来源：http://qna.andypj.xyz

[R62] 找最占空间的文件
来源：http://mxj.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://ghr.cheryme.top

[R63] 内存与进程
来源：http://mep.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://vqi.hesvh.cn

[R64] 结束进程
来源：http://izn.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://sra.hnqzz.top

[R65] 查看端口占用
来源：http://bvr.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tzm.svipenyu.cn

[R66] 定时任务
来源：http://iii.jqgufenzy.top

crontab -e;  crontab -l
来源：http://zfx.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://igy.dianchejie.cn

openssl rand -hex 16
来源：http://lzx.jiagoushi.top

[R68] 计算文件校验值
来源：http://iyo.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://kxl.havefunace.top

[R69] 生成随机密码
来源：http://iti.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://nzo.jiagoushi.top

[R70] 时间戳与互转
来源：http://ftz.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://wsf.cashguo.top

[R71] 日期格式化
来源：http://peo.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gdz.c1oappe.top

[R72] 等待端口就绪
来源：http://emo.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zrr.pycfn.com

[R73] 分割大日志
来源：http://xvo.sxryk.cn

split -l 1000 big.log part_
来源：http://gay.yfazqb.com

[R74] 批量重命名
来源：http://sqg.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://utx.yvedp.cn

[R75] 导出环境变量
来源：http://uan.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://cov.fehbvm.com

[R76] 使用临时文件
来源：http://hdg.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cbh.svipenyu.cn

[R77] 读取用户输入
来源：http://psm.chenlongwang.top

read -rp "请输入: " ans
来源：http://bcf.quarkkingdee.top

[R78] 交互式菜单
来源：http://xpz.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iiz.tian-w.cn

[R79] 解析命令行选项
来源：http://ldg.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fbj.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://tsy.fktsv.cn

time ./run.sh
来源：http://nva.hywenlv.cn

================================================================================
来源：http://uah.zdbjq.cn

S. C / C++ 专题
来源：http://qkt.jinqigufen.top

================================================================================
来源：http://tpx.cucudq.cn

[S01] C：Hello World
来源：http://vcl.zhongyouzk.top

#include <stdio.h>
来源：http://zwg.ydzc1.top


<!-- 参考信息 -->