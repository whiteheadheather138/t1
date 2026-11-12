代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pgl.wangdashe.top

[Q28] 求和与平均
来源：http://pia.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://czi.jianghu66.top

[Q29] 最大最小值
来源：http://gbp.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ieu.zhiwuduotai.top

[Q30] 分组统计
来源：http://zhi.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eie.cdnleiting.top

[Q31] 分组后过滤
来源：http://okf.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://skp.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://mxw.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ucw.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yyo.xinyue.icu

[Q33] 多列分组
来源：http://rmk.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nuv.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://rtn.hammf.cn

SELECT * FROM (
来源：http://ssq.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://smz.yonumen.top

) t WHERE rn = 1;
来源：http://ugb.jlsjyb.cn

[Q35] 内连接
来源：http://gxc.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lpz.zhijiandao.cn

[Q36] 左连接
来源：http://vke.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ean.jqgfzy.top

[Q37] 右连接
来源：http://ayt.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hgb.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://xmf.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wbm.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://atq.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gmd.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://chu.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nwp.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xne.dashuyun.cn

[Q41] 多表连接
来源：http://lpj.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ban.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://fki.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://fyr.ivvv.top

[Q42] 连接条件附加过滤
来源：http://zfw.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://poz.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://coi.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://xhe.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lfu.cucudq.cn

[Q44] IN 子查询
来源：http://ilx.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nvs.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://yvy.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qrv.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://wez.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sds.hysaishi.cn

[Q47] 与平均值比较
来源：http://dez.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mus.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://bsq.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dic.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://ryo.jqgfzy.top

[Q49] 更新单行
来源：http://uec.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cfy.fzhhl.top

[Q50] 批量更新
来源：http://jwv.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yso.tarul.cn

[Q51] 用子查询更新
来源：http://jxx.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iap.ppjwa.cn

[Q52] 删除指定行
来源：http://eba.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://bbm.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://spe.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xpc.sxryk.cn

[Q54] 清空表
来源：http://twv.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://ncc.epnwcf.com

[Q55] 排名（并列占位）
来源：http://bee.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blw.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://vvx.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ctf.fzhhl.top

[Q57] 行号
来源：http://nwx.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://brm.c1oappe.top

[Q58] 累计求和
来源：http://tcs.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tqi.chenjidiqi.icu

[Q59] 分组内累计
来源：http://mvz.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jud.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://drq.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzg.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vrf.xuanzx.com

[Q61] 移动平均
来源：http://rxk.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zxb.hongshengwenyu.top

[Q62] 分组占比
来源：http://mlt.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gmz.ehwqpu.com

[Q63] 开启事务
来源：http://kit.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://esc.zdqjudy.top

[Q64] 提交事务
来源：http://miz.yonumen.top

COMMIT;
来源：http://uxc.cucudq.cn

[Q65] 回滚事务
来源：http://dog.hnxiangtu.top

ROLLBACK;
来源：http://ppc.gogol.net.cn

[Q66] 行锁查询
来源：http://ddk.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xnc.snrcjt.cn

[Q67] 设置隔离级别
来源：http://jru.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bby.ydzc1.top

[Q68] 保存点
来源：http://jcx.hysaishi.cn

SAVEPOINT sp1;
来源：http://znr.yongpay.top

ROLLBACK TO sp1;
来源：http://yni.ppjwa.cn

[Q69] 查看执行计划
来源：http://swy.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hml.hammf.cn

[Q70] 更新统计信息
来源：http://aap.yueranfly.top

ANALYZE TABLE users;
来源：http://rio.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://ikj.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hcx.smart0.xyz

[Q72] 查看索引
来源：http://stg.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://yig.shuidangran.top

[Q73] 查看表状态
来源：http://sts.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://rmt.shzxlz.cn

[Q74] 强制使用索引
来源：http://yxm.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bum.nanxuanxn.top

[Q75] 日期格式化
来源：http://hbs.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kuk.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://siw.fzhhl.top

[Q76] 按天统计
来源：http://fcu.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nho.9152youxi.cn

[Q77] 时间加减
来源：http://cnm.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ezs.hcnkem.com

[Q78] 当前时间
来源：http://rvf.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xqd.epnwcf.com

[Q79] 字符串拼接
来源：http://guf.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yxp.hnqzz.top

[Q80] 字符串截取
来源：http://zbd.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xrf.jinqigfzy.top

[Q81] 字符串替换
来源：http://jfr.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xnm.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://qkg.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cfn.ydjk.org.cn

[Q83] 大小写转换
来源：http://nmh.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mzy.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://ijm.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://bxo.quarkkingdee.top

[Q85] 数值取整
来源：http://lub.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://utc.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://bqo.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kph.yj20258.top

[Q87] JSON 字段做条件
来源：http://urk.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrh.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://vti.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lca.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ych.gzhubu.top

[Q89] 判断表是否存在
来源：http://deg.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bdy.sysykeji.top

[Q90] 生成序号列
来源：http://uxx.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qfk.shanyushiyangkeji.top

================================================================================
来源：http://txr.zhijiandao.cn

R. Bash 专题
来源：http://cyw.yj20258.top

================================================================================
来源：http://ddl.yj202588.top

[R01] shebang 与严格模式
来源：http://zlr.epnwcf.com

#!/usr/bin/env bash
来源：http://pjn.aizwys.cn

set -euo pipefail
来源：http://ctn.havefunace.top

[R02] 变量赋值与使用
来源：http://tfg.ydzc1.top

name="Tom"; echo "$name"
来源：http://nfp.fengsongda.top

[R03] 只读变量
来源：http://akq.52xcode.cn

readonly PI=3.14
来源：http://wfy.zhoulong.xyz

[R04] 位置参数
来源：http://wcq.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgr.xuanzx.com

[R05] 参数默认值
来源：http://kca.feifeiyinyue.top

name="${1:-default}"
来源：http://jpr.yvedp.cn

[R06] 判断命令是否存在
来源：http://nmt.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vdi.hysaishi.cn

[R07] if 判断文件
来源：http://cba.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hlp.hammf.cn

[R08] 数值比较
来源：http://njf.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://oqy.iojbl.cn

[R09] 字符串比较
来源：http://koz.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yuf.yj202588.top

[R10] 正则匹配
来源：http://qct.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sti.kuanghao11.cn

[R11] case 多分支
来源：http://vkx.yuanzhike.top

case "$1" in
来源：http://rib.sxryk.cn

start) echo "启动" ;;
来源：http://arn.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://fad.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://skd.52xcode.cn

esac
来源：http://ijl.birdmap.top

[R12] for 遍历文件
来源：http://qxk.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://qiv.cucudq.cn

[R13] for 计数循环
来源：http://qpo.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://vcb.cashguo.top

[R14] C 风格 for
来源：http://lss.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lzz.daria6918.cn

[R15] while 逐行读文件
来源：http://kfk.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uwb.bjfxy.top

[R16] until 等待条件
来源：http://ood.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://itn.jqgufenzy.top

[R17] 数组定义与取值
来源：http://kzs.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://cau.daxiang520.top

[R18] 遍历数组
来源：http://hsx.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ewm.52xcode.cn

[R19] 数组长度
来源：http://dty.aizwys.cn

echo "${#arr[@]}"
来源：http://qic.xuanzx.com

[R20] 关联数组（字典）
来源：http://hvy.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qpn.hnqzz.top

[R21] 字符串长度
来源：http://pyy.shanyushiyangtech.top

echo "${#s}"
来源：http://hsf.sjlbkw.cn

[R22] 截取子串
来源：http://zkh.zhengqikj.top

echo "${s:0:5}"
来源：http://gpj.jinqigfzy.top

[R23] 字符串替换
来源：http://kcs.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rda.yuxming.cn

[R24] 大小写转换
来源：http://hfb.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://vtk.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://axi.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dzo.birdmap.top

[R26] 命令替换
来源：http://rde.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://wnx.zdbjq.cn

[R27] 算术展开
来源：http://ckl.fzhhl.top

echo $((1 + 2 * 3))
来源：http://ktf.chenlongwang.top

[R28] 浮点运算
来源：http://hob.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://dbq.ehwqpu.com

[R29] 定义函数
来源：http://ogk.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xsc.bjfxy.top

[R30] 函数返回状态码
来源：http://war.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://lug.smart0.xyz

[R31] 局部变量
来源：http://ldo.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://bdg.chenzaomai.com

[R32] 参数个数校验
来源：http://sya.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cin.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://qpb.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mxl.yueranfly.top

[R34] 退出时清理
来源：http://uht.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jlx.fzhhl.top

[R35] 后台执行并等待
来源：http://rya.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wou.fzhhl.top

[R36] 并发执行多个任务
来源：http://ryf.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uoc.9152youxi.cn

[R37] 把输出赋给变量
来源：http://zxr.hnqzz.top

files=$(ls -1)
来源：http://asa.cucudq.cn

[R38] 管道串联
来源：http://iyn.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://xjv.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://sen.fehbvm.com

cmd > out.log 2>&1
来源：http://jgx.dianchejie.cn

[R40] 追加写日志
来源：http://dxu.bjfxy.top

echo "log" >> out.log
来源：http://vby.hcnkem.com

[R41] 丢弃输出
来源：http://mpw.ivvv.top

cmd >/dev/null 2>&1
来源：http://jfv.wangshuangyany.cn

[R42] 输入重定向
来源：http://vto.zhiwuduotai.top

wc -l < a.txt
来源：http://bvr.zycfv.cn

[R43] 按名字查找文件
来源：http://mgu.snrcjt.cn

find . -name "*.log" -type f
来源：http://gbg.xinyue.icu

[R44] 按修改时间查找
来源：http://rfz.zhengqikj.top

find . -mtime -7 -type f
来源：http://sbs.cheryme.top

[R45] 批量删除
来源：http://bcl.xinyue.icu

find . -name "*.tmp" -delete
来源：http://gsg.xziqi.cn

[R46] 递归替换文件内容
来源：http://xek.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pbh.yongpay.top

[R47] sed 单行替换
来源：http://yug.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bif.tian-w.cn

[R48] awk 取指定列
来源：http://ufl.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://sxo.yanxiufei.cn

[R49] awk 带条件
来源：http://ipi.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vwy.shzxlz.cn

[R50] awk 求和
来源：http://jwh.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://mdw.zycfv.cn

[R51] 排序去重取前几
来源：http://yfu.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sdv.yj202588.top

[R52] 统计行数
来源：http://rpz.yfazqb.com

wc -l a.txt
来源：http://one.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://wpk.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ind.yuanzhike.top

[R54] 比较两个文件
来源：http://anx.ydzc1.top

diff a.txt b.txt
来源：http://lms.shangyingyoupin.top

[R55] 压缩与解压
来源：http://tbh.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aij.yvedp.cn

[R56] 远程拷贝
来源：http://vex.zdbjq.cn

scp file user@host:/path/
来源：http://mvr.zhixingplan.top

[R57] 远程执行命令
来源：http://urz.dianchejie.cn

ssh user@host 'uptime'
来源：http://tqg.jqgfzy.top

[R58] 下载文件
来源：http://gds.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tmx.xziqi.cn

[R59] 发 POST JSON
来源：http://mxt.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hey.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://jbv.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sqj.hysaishi.cn

[R61] 磁盘占用
来源：http://nrs.daria6918.cn

df -h;  du -sh *
来源：http://zby.c1oappe.top

[R62] 找最占空间的文件
来源：http://ate.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://nmu.zhiwuduotai.top

[R63] 内存与进程
来源：http://qxl.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://kcy.tarul.cn

[R64] 结束进程
来源：http://sxg.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://gvn.wangdashe.top

[R65] 查看端口占用
来源：http://xok.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://utb.cheryme.top

[R66] 定时任务
来源：http://mnu.hnxiangtu.top

crontab -e;  crontab -l
来源：http://ykt.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://nro.dashuyun.cn

openssl rand -hex 16
来源：http://hhm.ppjwa.cn

[R68] 计算文件校验值
来源：http://kmy.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://qvr.ybcxt.top

[R69] 生成随机密码
来源：http://ytd.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://dwz.havefunace.top

[R70] 时间戳与互转
来源：http://jjm.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://oai.fktsv.cn

[R71] 日期格式化
来源：http://dnm.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oem.ydzc1.top

[R72] 等待端口就绪
来源：http://lkj.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yyn.hongshengwenyu.top

[R73] 分割大日志
来源：http://kgr.ppjwa.cn

split -l 1000 big.log part_
来源：http://knb.nanxinkj.top

[R74] 批量重命名
来源：http://aqb.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyq.iojbl.cn

[R75] 导出环境变量
来源：http://sbv.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://qah.yj20258888.top

[R76] 使用临时文件
来源：http://zug.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wyv.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://olz.xylfe.cn


<!-- 参考信息 -->