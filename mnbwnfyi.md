代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wlw.cucudq.cn

[Q28] 求和与平均
来源：http://bsc.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vkg.tian-w.cn

[Q29] 最大最小值
来源：http://bsz.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bfl.dianchejie.cn

[Q30] 分组统计
来源：http://jmz.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyb.zhengqikj.top

[Q31] 分组后过滤
来源：http://miq.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://amj.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://rpb.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xbs.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pth.redwolf501.top

[Q33] 多列分组
来源：http://itq.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lek.yangfankeji.com

[Q34] 每组取第一条
来源：http://pwy.jinqigufen.top

SELECT * FROM (
来源：http://yck.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovb.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://edw.sufxvd.cn

[Q35] 内连接
来源：http://rop.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ari.shanyushiyangtech.top

[Q36] 左连接
来源：http://zmt.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hmf.jlsjyb.cn

[Q37] 右连接
来源：http://wgm.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pyo.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://hzc.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qbb.yonumen.top

[Q39] 自连接（查上下级）
来源：http://ryr.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jhn.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kjx.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wpu.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vwr.pycfn.com

[Q41] 多表连接
来源：http://ilc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bqy.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://tas.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://bdk.havefunace.top

[Q42] 连接条件附加过滤
来源：http://pxv.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://hth.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tmi.sweek.top

[Q43] 标量子查询
来源：http://bqh.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ofl.gzhubu.top

[Q44] IN 子查询
来源：http://hhs.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jqs.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://wnp.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jka.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://znf.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hox.shuidangran.top

[Q47] 与平均值比较
来源：http://kys.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rbs.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ryj.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rvr.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://nxe.guannengcc.top

[Q49] 更新单行
来源：http://wqw.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kay.sysykeji.top

[Q50] 批量更新
来源：http://yqh.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftt.cqqwz.cn

[Q51] 用子查询更新
来源：http://cdp.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://esk.dianchejie.cn

[Q52] 删除指定行
来源：http://egw.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://kwu.yfazqb.com

[Q53] 按条件删除
来源：http://pqa.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hyv.jinqigufen.top

[Q54] 清空表
来源：http://niv.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://wim.hammf.cn

[Q55] 排名（并列占位）
来源：http://agh.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hou.kuanghao11.cn

[Q56] 密集排名（并列不占位）
来源：http://kbh.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://phm.zhijiandao.cn

[Q57] 行号
来源：http://kjp.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wnn.yongpay.top

[Q58] 累计求和
来源：http://xln.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zmr.iojbl.cn

[Q59] 分组内累计
来源：http://emh.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ibo.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://qth.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kdy.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jes.jlsjyb.cn

[Q61] 移动平均
来源：http://yql.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ljq.ybcxt.top

[Q62] 分组占比
来源：http://bku.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uvv.fengsongda.top

[Q63] 开启事务
来源：http://mue.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nyd.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://nnl.feifeiyinyue.top

COMMIT;
来源：http://okk.yj202588.top

[Q65] 回滚事务
来源：http://lfs.nanxinkj.top

ROLLBACK;
来源：http://vew.vehdjk.com

[Q66] 行锁查询
来源：http://gyq.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ylo.fengsongda.top

[Q67] 设置隔离级别
来源：http://kun.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tnt.jinghuilouyu.cn

[Q68] 保存点
来源：http://wsb.jqgfzy.top

SAVEPOINT sp1;
来源：http://jjz.zdbjq.cn

ROLLBACK TO sp1;
来源：http://pde.daria6918.cn

[Q69] 查看执行计划
来源：http://poi.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zrp.mhx1999.top

[Q70] 更新统计信息
来源：http://dpm.xinyue.icu

ANALYZE TABLE users;
来源：http://yxg.yfazqb.com

[Q71] 查看建表语句
来源：http://eqy.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qtf.0kj1m.cn

[Q72] 查看索引
来源：http://fkl.sweek.top

SHOW INDEX FROM users;
来源：http://nox.zycfv.cn

[Q73] 查看表状态
来源：http://udg.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rap.sweek.top

[Q74] 强制使用索引
来源：http://xio.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pdl.kuanghao11.cn

[Q75] 日期格式化
来源：http://jtp.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mop.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dyj.zhongyouzk.top

[Q76] 按天统计
来源：http://hqa.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://okm.yonumen.top

[Q77] 时间加减
来源：http://oru.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fwh.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://dix.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://olg.iojbl.cn

[Q79] 字符串拼接
来源：http://vqa.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uhe.zdqjudy.top

[Q80] 字符串截取
来源：http://jzx.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xdk.yonumen.top

[Q81] 字符串替换
来源：http://gvt.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://plo.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://dvy.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://crd.mhx1999.top

[Q83] 大小写转换
来源：http://yjv.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nnp.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://klq.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://mkb.aizwys.cn

[Q85] 数值取整
来源：http://hgj.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gfi.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://xld.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vmd.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://myn.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ftm.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://lqb.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aog.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pjx.svipenyu.cn

[Q89] 判断表是否存在
来源：http://zkr.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ott.cdnleiting.top

[Q90] 生成序号列
来源：http://zab.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xak.fengsongda.top

================================================================================
来源：http://soi.c1oappe.top

R. Bash 专题
来源：http://jtb.havefunace.top

================================================================================
来源：http://lct.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://odc.hnqzz.top

#!/usr/bin/env bash
来源：http://dtw.snrcjt.cn

set -euo pipefail
来源：http://ods.zdbjq.cn

[R02] 变量赋值与使用
来源：http://uhn.jiagoushi.top

name="Tom"; echo "$name"
来源：http://ewa.jianghu66.top

[R03] 只读变量
来源：http://qqb.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://vye.ivvv.top

[R04] 位置参数
来源：http://itf.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://low.cdnleiting.top

[R05] 参数默认值
来源：http://qcc.yanxiufei.cn

name="${1:-default}"
来源：http://hyo.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://hba.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://snl.tarul.cn

[R07] if 判断文件
来源：http://zqh.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://htn.yuanzhike.top

[R08] 数值比较
来源：http://qgf.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hhd.cdnleiting.top

[R09] 字符串比较
来源：http://tgv.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ulo.hesvh.cn

[R10] 正则匹配
来源：http://fwf.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mvw.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://zzf.nanxuanxn.top

case "$1" in
来源：http://qlp.hnqzz.top

start) echo "启动" ;;
来源：http://qcx.hywenlv.cn

stop)  echo "停止" ;;
来源：http://mac.xziqi.cn

*)     echo "未知命令" ;;
来源：http://dek.gzhubu.top

esac
来源：http://rfa.hongshengwenyu.top

[R12] for 遍历文件
来源：http://rqt.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://znw.zhoulong.xyz

[R13] for 计数循环
来源：http://iww.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://cvy.svipenyu.cn

[R14] C 风格 for
来源：http://zis.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iuw.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://vsc.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nlx.meibo888.top

[R16] until 等待条件
来源：http://aht.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rjp.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://oyh.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://hsf.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://ehd.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tdb.tanke756.top

[R19] 数组长度
来源：http://toz.52xcode.cn

echo "${#arr[@]}"
来源：http://qqa.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://xfa.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://umj.ybcxt.top

[R21] 字符串长度
来源：http://oxz.ydzc1.top

echo "${#s}"
来源：http://qar.zhaomingkeji.xyz

[R22] 截取子串
来源：http://ump.fehbvm.com

echo "${s:0:5}"
来源：http://zen.xuetiantiany.cn

[R23] 字符串替换
来源：http://znt.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aoa.dashuyun.cn

[R24] 大小写转换
来源：http://wao.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dof.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://eml.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lli.xuetiantiany.cn

[R26] 命令替换
来源：http://cti.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://fcu.shanyushiyangkeji.top

[R27] 算术展开
来源：http://tzm.havefunace.top

echo $((1 + 2 * 3))
来源：http://fdh.ppjwa.cn

[R28] 浮点运算
来源：http://vcm.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://yqv.fzhhl.top

[R29] 定义函数
来源：http://daw.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jjp.fktsv.cn

[R30] 函数返回状态码
来源：http://fuq.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://ced.nanxinkj.top

[R31] 局部变量
来源：http://eul.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://ghi.ybcxt.top

[R32] 参数个数校验
来源：http://tvj.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sec.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://asn.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvd.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://hqa.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://swq.sysykeji.top

[R35] 后台执行并等待
来源：http://ckp.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xza.cdnleiting.top

[R36] 并发执行多个任务
来源：http://gtk.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://csn.snrcjt.cn

[R37] 把输出赋给变量
来源：http://jfh.yj20258888.top

files=$(ls -1)
来源：http://gof.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://flq.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://vnn.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://bsu.ydjk.org.cn

cmd > out.log 2>&1
来源：http://cdd.shuidangran.top

[R40] 追加写日志
来源：http://orn.ctjpmb.com

echo "log" >> out.log
来源：http://mtd.xylfe.cn

[R41] 丢弃输出
来源：http://wwf.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://rsz.zhongyouzk.top

[R42] 输入重定向
来源：http://njd.jyoumei.cn

wc -l < a.txt
来源：http://jvt.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://adz.yanxiufei.cn

find . -name "*.log" -type f
来源：http://jto.yongpay.top

[R44] 按修改时间查找
来源：http://dcw.c1oappe.top

find . -mtime -7 -type f
来源：http://gjy.snrcjt.cn

[R45] 批量删除
来源：http://mru.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://vkx.guannengcc.top

[R46] 递归替换文件内容
来源：http://zwk.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pnb.xinyue.icu

[R47] sed 单行替换
来源：http://gny.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://mtf.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://tum.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://ehs.tian-w.cn

[R49] awk 带条件
来源：http://sjf.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gqe.gaohongyu789.top

[R50] awk 求和
来源：http://xoj.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://abd.andypj.xyz

[R51] 排序去重取前几
来源：http://idr.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ewe.cdnleiting.top

[R52] 统计行数
来源：http://jor.xuetiantiany.cn

wc -l a.txt
来源：http://ehl.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://olp.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fcm.gzhubu.top

[R54] 比较两个文件
来源：http://evf.ydjk.org.cn

diff a.txt b.txt
来源：http://xap.quarkkingdee.top

[R55] 压缩与解压
来源：http://vfm.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kas.xuanzx.com

[R56] 远程拷贝
来源：http://fvn.birdmap.top

scp file user@host:/path/
来源：http://wqj.snrcjt.cn

[R57] 远程执行命令
来源：http://vwc.daria6918.cn

ssh user@host 'uptime'
来源：http://jtd.chenjidiqi.icu

[R58] 下载文件
来源：http://miz.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oyx.xylfe.cn

[R59] 发 POST JSON
来源：http://zui.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wrj.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://pzi.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yxe.yangfankeji.com

[R61] 磁盘占用
来源：http://bkd.gogol.net.cn

df -h;  du -sh *
来源：http://sqg.fzhhl.top

[R62] 找最占空间的文件
来源：http://xwo.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://bxr.daxiang520.top

[R63] 内存与进程
来源：http://esb.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://ffu.ehwqpu.com

[R64] 结束进程
来源：http://uat.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://nal.ppjwa.cn

[R65] 查看端口占用
来源：http://hgo.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://brk.tian-w.cn

[R66] 定时任务
来源：http://guu.zycfv.cn

crontab -e;  crontab -l
来源：http://igc.hammf.cn

[R67] 生成随机十六进制串
来源：http://jbn.ppjwa.cn

openssl rand -hex 16
来源：http://gyq.xuanzx.com

[R68] 计算文件校验值
来源：http://qtx.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://adv.pycfn.com

[R69] 生成随机密码
来源：http://ael.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://zct.snrcjt.cn

[R70] 时间戳与互转
来源：http://aie.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://tka.wangshuangyany.cn

[R71] 日期格式化
来源：http://jda.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://gpj.hesvh.cn

[R72] 等待端口就绪
来源：http://euv.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://syg.shanyushiyangtech.top

[R73] 分割大日志
来源：http://okn.aizwys.cn

split -l 1000 big.log part_
来源：http://wgf.cashguo.top

[R74] 批量重命名
来源：http://jqr.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xvj.daria6918.cn

[R75] 导出环境变量
来源：http://siv.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://fah.shzxlz.cn

[R76] 使用临时文件
来源：http://pjn.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://edm.hammf.cn

[R77] 读取用户输入
来源：http://egh.sweek.top


<!-- 参考信息 -->