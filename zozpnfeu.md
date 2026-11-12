代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dsy.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://fje.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://swx.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uwp.jyoumei.cn

[Q33] 多列分组
来源：http://vyi.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://isx.cucudq.cn

[Q34] 每组取第一条
来源：http://pqn.uphjek.com

SELECT * FROM (
来源：http://uwr.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zym.cheryme.top

) t WHERE rn = 1;
来源：http://zze.tian-w.cn

[Q35] 内连接
来源：http://hem.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://njq.meibo888.top

[Q36] 左连接
来源：http://lcx.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://omf.9152youxi.cn

[Q37] 右连接
来源：http://qvi.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://khi.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://mct.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://plt.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://xzz.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://itx.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bam.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ibx.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xip.zhijiandao.cn

[Q41] 多表连接
来源：http://gje.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dxz.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://vlp.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://huu.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://hux.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://vnx.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ofc.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://fmy.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lfl.wangshuangyany.cn

[Q44] IN 子查询
来源：http://kmk.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xjy.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://qry.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lzm.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vyu.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rua.hysaishi.cn

[Q47] 与平均值比较
来源：http://moc.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rff.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://uji.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mgr.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://klw.iojbl.cn

[Q49] 更新单行
来源：http://cck.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mlm.chenzaomai.com

[Q50] 批量更新
来源：http://lmc.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gao.smart0.xyz

[Q51] 用子查询更新
来源：http://uig.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lxf.gaohongyu789.top

[Q52] 删除指定行
来源：http://kmu.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://kyq.sysykeji.top

[Q53] 按条件删除
来源：http://mlt.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dpz.zhiwuduotai.top

[Q54] 清空表
来源：http://agm.hcnkem.com

TRUNCATE TABLE logs;
来源：http://orh.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://faw.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aax.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://flg.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wrh.birdmap.top

[Q57] 行号
来源：http://zzn.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ivs.yueranfly.top

[Q58] 累计求和
来源：http://zea.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xss.yj20258.top

[Q59] 分组内累计
来源：http://lar.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dam.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://iba.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gln.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nhl.yonumen.top

[Q61] 移动平均
来源：http://ieb.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ayb.chenzaomai.com

[Q62] 分组占比
来源：http://hsn.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://avp.hesvh.cn

[Q63] 开启事务
来源：http://pyc.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nai.nwbrower.top

[Q64] 提交事务
来源：http://rsy.yj20258.top

COMMIT;
来源：http://oxw.zhoulong.xyz

[Q65] 回滚事务
来源：http://qum.yangfankeji.com

ROLLBACK;
来源：http://xzj.pengpengdd.cyou

[Q66] 行锁查询
来源：http://hva.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ngq.snrcjt.cn

[Q67] 设置隔离级别
来源：http://vkx.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bbm.jinghuilouyu.cn

[Q68] 保存点
来源：http://wki.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://gkf.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://oop.yfazqb.com

[Q69] 查看执行计划
来源：http://fzx.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wlx.shuidangran.top

[Q70] 更新统计信息
来源：http://vxm.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://suz.chenlongwang.top

[Q71] 查看建表语句
来源：http://wwh.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qcu.guannengcc.top

[Q72] 查看索引
来源：http://cpl.hammf.cn

SHOW INDEX FROM users;
来源：http://pnt.uphjek.com

[Q73] 查看表状态
来源：http://qtz.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://qwi.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://fcg.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jeh.dianchejie.cn

[Q75] 日期格式化
来源：http://qds.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ucf.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://myh.svipenyu.cn

[Q76] 按天统计
来源：http://gki.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vhj.nanxinkj.top

[Q77] 时间加减
来源：http://ejc.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppo.hysaishi.cn

[Q78] 当前时间
来源：http://kcv.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zkf.sweek.top

[Q79] 字符串拼接
来源：http://vny.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://buu.daxiang520.top

[Q80] 字符串截取
来源：http://umc.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qko.chenzaomai.com

[Q81] 字符串替换
来源：http://azg.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lif.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://cqw.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nod.nwbrower.top

[Q83] 大小写转换
来源：http://tnn.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fwd.sufxvd.cn

[Q84] 去除首尾空格
来源：http://mco.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://zlj.dianchejie.cn

[Q85] 数值取整
来源：http://hhy.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bhs.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://zly.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yvn.yuxming.cn

[Q87] JSON 字段做条件
来源：http://cah.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kyd.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://urw.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eaq.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tet.cqqwz.cn

[Q89] 判断表是否存在
来源：http://pxn.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eev.smart0.xyz

[Q90] 生成序号列
来源：http://pvy.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tmt.aizwys.cn

================================================================================
来源：http://dkr.zdbjq.cn

R. Bash 专题
来源：http://ife.shanyushiyangtech.top

================================================================================
来源：http://dtm.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://bcp.nanxuanxn.top

#!/usr/bin/env bash
来源：http://gzv.yanxiufei.cn

set -euo pipefail
来源：http://adu.zdqjudy.top

[R02] 变量赋值与使用
来源：http://xxz.fengsongda.top

name="Tom"; echo "$name"
来源：http://zxp.quarkkingdee.top

[R03] 只读变量
来源：http://qwq.xuetiantiany.cn

readonly PI=3.14
来源：http://txc.shangyingyoupin.top

[R04] 位置参数
来源：http://ktb.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smv.yuanzhike.top

[R05] 参数默认值
来源：http://gfd.yueranfly.top

name="${1:-default}"
来源：http://inl.xuanzx.com

[R06] 判断命令是否存在
来源：http://qnu.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wlr.cdnleiting.top

[R07] if 判断文件
来源：http://jys.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ixx.daxiang520.top

[R08] 数值比较
来源：http://nyj.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ugk.chenzaomai.com

[R09] 字符串比较
来源：http://wdv.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jpz.316326.xyz

[R10] 正则匹配
来源：http://jbd.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://laf.jinqigufen.top

[R11] case 多分支
来源：http://ajj.shangyingyoupin.top

case "$1" in
来源：http://fsh.yj20258.top

start) echo "启动" ;;
来源：http://duk.guannengcc.top

stop)  echo "停止" ;;
来源：http://whs.yuxming.cn

*)     echo "未知命令" ;;
来源：http://kky.yj20258888.top

esac
来源：http://fhk.gzhubu.top

[R12] for 遍历文件
来源：http://tiv.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://iia.quarkkingdee.top

[R13] for 计数循环
来源：http://sak.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://qkv.cashguo.top

[R14] C 风格 for
来源：http://ezn.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vqz.ybcxt.top

[R15] while 逐行读文件
来源：http://kxf.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sbf.cqqwz.cn

[R16] until 等待条件
来源：http://agu.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://arx.xziqi.cn

[R17] 数组定义与取值
来源：http://lgm.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pmf.kuanghao11.cn

[R18] 遍历数组
来源：http://mrn.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fcg.epnwcf.com

[R19] 数组长度
来源：http://oco.yj202588.top

echo "${#arr[@]}"
来源：http://sqd.nanxinkj.top

[R20] 关联数组（字典）
来源：http://ikg.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uhd.xylfe.cn

[R21] 字符串长度
来源：http://qpg.fehbvm.com

echo "${#s}"
来源：http://psd.wangshuangyany.cn

[R22] 截取子串
来源：http://otc.andypj.xyz

echo "${s:0:5}"
来源：http://gxc.haohaochexian.top

[R23] 字符串替换
来源：http://ycq.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bjw.yonumen.top

[R24] 大小写转换
来源：http://nej.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bpr.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://ihc.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vlx.yueranfly.top

[R26] 命令替换
来源：http://jmv.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://etq.fengsongda.top

[R27] 算术展开
来源：http://dft.fktsv.cn

echo $((1 + 2 * 3))
来源：http://ibt.cqqwz.cn

[R28] 浮点运算
来源：http://vfu.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://frc.iojbl.cn

[R29] 定义函数
来源：http://vnt.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://khc.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://gqe.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://eil.hnqzz.top

[R31] 局部变量
来源：http://kbp.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://jfk.yongpay.top

[R32] 参数个数校验
来源：http://pnr.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tke.cheryme.top

[R33] 捕获错误并提示行号
来源：http://eay.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zkh.quarkkingdee.top

[R34] 退出时清理
来源：http://swi.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://akm.ybcxt.top

[R35] 后台执行并等待
来源：http://cdh.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qpm.vehdjk.com

[R36] 并发执行多个任务
来源：http://zmk.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mme.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://llz.sufxvd.cn

files=$(ls -1)
来源：http://qou.hfpthk.cn

[R38] 管道串联
来源：http://lub.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://kxp.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://wcy.gotoacloud.top

cmd > out.log 2>&1
来源：http://ytb.cashguo.top

[R40] 追加写日志
来源：http://pfq.iojbl.cn

echo "log" >> out.log
来源：http://puw.redwolf501.top

[R41] 丢弃输出
来源：http://yvy.aizwys.cn

cmd >/dev/null 2>&1
来源：http://wlm.gotoacloud.top

[R42] 输入重定向
来源：http://rjf.yuanzhike.top

wc -l < a.txt
来源：http://qyj.cqqwz.cn

[R43] 按名字查找文件
来源：http://nzy.yueranfly.top

find . -name "*.log" -type f
来源：http://pwn.hesvh.cn

[R44] 按修改时间查找
来源：http://ahf.fzhhl.top

find . -mtime -7 -type f
来源：http://tqp.cdnleiting.top

[R45] 批量删除
来源：http://duv.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://vqw.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://xle.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzn.andypj.xyz

[R47] sed 单行替换
来源：http://zfj.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://brl.sjlbkw.cn

[R48] awk 取指定列
来源：http://fvz.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://aoh.ppjwa.cn

[R49] awk 带条件
来源：http://odz.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pbl.hcnkem.com

[R50] awk 求和
来源：http://prd.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://mlc.316326.xyz

[R51] 排序去重取前几
来源：http://vvx.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wiw.yangfankeji.com

[R52] 统计行数
来源：http://gwu.yangfankeji.com

wc -l a.txt
来源：http://vtq.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://ptz.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wtq.zycfv.cn

[R54] 比较两个文件
来源：http://now.iojbl.cn

diff a.txt b.txt
来源：http://vxc.feifeiyinyue.top

[R55] 压缩与解压
来源：http://obk.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fiu.c1oappe.top

[R56] 远程拷贝
来源：http://pmd.daxiang520.top

scp file user@host:/path/
来源：http://oki.uphjek.com

[R57] 远程执行命令
来源：http://thl.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://xoq.yueranfly.top

[R58] 下载文件
来源：http://djv.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://drc.mhx1999.top

[R59] 发 POST JSON
来源：http://kgo.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mqe.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://cow.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hym.ehwqpu.com

[R61] 磁盘占用
来源：http://zne.zhixingplan.top

df -h;  du -sh *
来源：http://vni.ppjwa.cn

[R62] 找最占空间的文件
来源：http://arj.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://lkh.dianchejie.cn

[R63] 内存与进程
来源：http://nwx.ivvv.top

free -h;  ps aux | grep nginx
来源：http://iko.mhx1999.top

[R64] 结束进程
来源：http://vri.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://tjn.kuanghao11.cn

[R65] 查看端口占用
来源：http://psw.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rwe.gotoacloud.top

[R66] 定时任务
来源：http://nkg.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://bxu.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://hmc.gotoacloud.top

openssl rand -hex 16
来源：http://mql.chenlongwang.top

[R68] 计算文件校验值
来源：http://oro.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://cof.wangshuangyany.cn

[R69] 生成随机密码
来源：http://rqs.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://evp.aizwys.cn

[R70] 时间戳与互转
来源：http://vat.xylfe.cn

date +%s;  date -d @1700000000
来源：http://yld.yj20258.top

[R71] 日期格式化
来源：http://bry.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://stc.yuanzhike.top

[R72] 等待端口就绪
来源：http://gyq.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rgu.yanxiufei.cn

[R73] 分割大日志
来源：http://kal.haohaochexian.top

split -l 1000 big.log part_
来源：http://jix.yueranfly.top

[R74] 批量重命名
来源：http://wuq.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cfj.yj20258.top

[R75] 导出环境变量
来源：http://rid.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://kis.vqdsnc.cn

[R76] 使用临时文件
来源：http://mlj.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emm.ydzc1.top

[R77] 读取用户输入
来源：http://uxv.shuidangran.top

read -rp "请输入: " ans
来源：http://uor.ivvv.top

[R78] 交互式菜单
来源：http://dzt.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jxb.mhx1999.top

[R79] 解析命令行选项
来源：http://ktb.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wmh.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://xdo.sxryk.cn

time ./run.sh
来源：http://rss.hfpthk.cn

================================================================================
来源：http://hkq.c1oappe.top


<!-- 参考信息 -->