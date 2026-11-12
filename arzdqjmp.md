代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wgo.birdmap.top

[Q26] 计数
来源：http://yrx.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://pyg.fzhhl.top

[Q27] 条件计数
来源：http://slu.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cfb.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://kup.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qjm.sweek.top

[Q29] 最大最小值
来源：http://jdd.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://kco.jyoumei.cn

[Q30] 分组统计
来源：http://cok.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wkm.hammf.cn

[Q31] 分组后过滤
来源：http://qrl.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fsf.fengsongda.top

[Q32] 分组拼接字符串
来源：http://zjm.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tmr.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mfe.shzxlz.cn

[Q33] 多列分组
来源：http://dna.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ocq.guannengcc.top

[Q34] 每组取第一条
来源：http://tzc.hcnkem.com

SELECT * FROM (
来源：http://gff.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://alr.zycfv.cn

) t WHERE rn = 1;
来源：http://bsd.pengpengdd.cyou

[Q35] 内连接
来源：http://peh.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tiw.iojbl.cn

[Q36] 左连接
来源：http://ktf.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://toj.cqqwz.cn

[Q37] 右连接
来源：http://hzu.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vja.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mqg.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qhc.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://juf.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ubo.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bei.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ktm.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ztl.meibo888.top

[Q41] 多表连接
来源：http://zka.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sun.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://hdo.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://ozq.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://iwn.birdmap.top

SELECT u.name, o.amount FROM users u
来源：http://bxr.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xqq.yj20258.top

[Q43] 标量子查询
来源：http://mve.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hut.dashuyun.cn

[Q44] IN 子查询
来源：http://gwq.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vem.yongpay.top

[Q45] EXISTS 判断存在
来源：http://tlv.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ecu.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://bvb.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sro.zhixingplan.top

[Q47] 与平均值比较
来源：http://bhy.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://san.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://non.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tgg.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://mhf.zdqjudy.top

[Q49] 更新单行
来源：http://yir.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwh.hammf.cn

[Q50] 批量更新
来源：http://tba.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ilk.dashuyun.cn

[Q51] 用子查询更新
来源：http://pyx.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btk.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://svt.svipenyu.cn

DELETE FROM users WHERE id = 10;
来源：http://gku.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://poe.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pra.zycfv.cn

[Q54] 清空表
来源：http://zty.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://ivi.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://vcl.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ykk.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://gtc.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tan.aibaodan.cn

[Q57] 行号
来源：http://qfy.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yht.bjfxy.top

[Q58] 累计求和
来源：http://ikt.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dle.ehwqpu.com

[Q59] 分组内累计
来源：http://nxe.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jay.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://mgp.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zsj.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://max.xylfe.cn

[Q61] 移动平均
来源：http://nhn.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qdq.ctjpmb.com

[Q62] 分组占比
来源：http://txw.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://htf.yvedp.cn

[Q63] 开启事务
来源：http://ubj.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cvx.fzhhl.top

[Q64] 提交事务
来源：http://cxf.aizwys.cn

COMMIT;
来源：http://stx.sufxvd.cn

[Q65] 回滚事务
来源：http://kad.shanyushiyangkeji.top

ROLLBACK;
来源：http://jnr.tianlin.xyz

[Q66] 行锁查询
来源：http://siy.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ihr.9152youxi.cn

[Q67] 设置隔离级别
来源：http://dsv.chenjidiqi.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://std.aizwys.cn

[Q68] 保存点
来源：http://nmw.zhongyouzk.top

SAVEPOINT sp1;
来源：http://jjm.guannengcc.top

ROLLBACK TO sp1;
来源：http://lwh.guannengcc.top

[Q69] 查看执行计划
来源：http://dnt.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zjh.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://csu.dashuyun.cn

ANALYZE TABLE users;
来源：http://enr.yueranfly.top

[Q71] 查看建表语句
来源：http://twy.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tfa.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://xhw.fktsv.cn

SHOW INDEX FROM users;
来源：http://xgg.hnqzz.top

[Q73] 查看表状态
来源：http://ugy.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gwj.guannengcc.top

[Q74] 强制使用索引
来源：http://xdk.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dxh.tarul.cn

[Q75] 日期格式化
来源：http://xnr.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qas.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tpw.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://zti.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vrj.0kj1m.cn

[Q77] 时间加减
来源：http://jgh.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zse.chenjidiqi.icu

[Q78] 当前时间
来源：http://afn.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vpf.pycfn.com

[Q79] 字符串拼接
来源：http://arb.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lcv.tanke756.top

[Q80] 字符串截取
来源：http://rpj.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tni.daxiang520.top

[Q81] 字符串替换
来源：http://rpz.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://npe.tarul.cn

[Q82] 字符长度与字节长度
来源：http://evs.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tcy.yuxming.cn

[Q83] 大小写转换
来源：http://tpm.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eeu.tarul.cn

[Q84] 去除首尾空格
来源：http://bie.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://ded.zhengqikj.top

[Q85] 数值取整
来源：http://tdx.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kme.havefunace.top

[Q86] 读取 JSON 字段
来源：http://txj.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mux.zycfv.cn

[Q87] JSON 字段做条件
来源：http://fft.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://myw.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://jix.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jma.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yvc.hammf.cn

[Q89] 判断表是否存在
来源：http://iut.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dvi.chenlongwang.top

[Q90] 生成序号列
来源：http://cxm.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dts.zdqjudy.top

================================================================================
来源：http://njn.yonumen.top

R. Bash 专题
来源：http://qul.tarul.cn

================================================================================
来源：http://glj.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://uwy.andypj.xyz

#!/usr/bin/env bash
来源：http://hqq.cqqwz.cn

set -euo pipefail
来源：http://ohq.bbcook.cn

[R02] 变量赋值与使用
来源：http://hye.dashuyun.cn

name="Tom"; echo "$name"
来源：http://ejp.jqgfzy.top

[R03] 只读变量
来源：http://igo.yvedp.cn

readonly PI=3.14
来源：http://zrd.svipenyu.cn

[R04] 位置参数
来源：http://oll.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vsp.smart0.xyz

[R05] 参数默认值
来源：http://kzq.gzhubu.top

name="${1:-default}"
来源：http://isp.cdnleiting.top

[R06] 判断命令是否存在
来源：http://bpo.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://add.yangfankeji.com

[R07] if 判断文件
来源：http://pmy.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://alj.yuanzhike.top

[R08] 数值比较
来源：http://uos.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dkq.pengpengdd.cyou

[R09] 字符串比较
来源：http://exr.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvu.hfpthk.cn

[R10] 正则匹配
来源：http://abr.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dpa.yuanzhike.top

[R11] case 多分支
来源：http://ufq.jqgufenzy.top

case "$1" in
来源：http://lar.jyoumei.cn

start) echo "启动" ;;
来源：http://njf.9152youxi.cn

stop)  echo "停止" ;;
来源：http://xbk.yongpay.top

*)     echo "未知命令" ;;
来源：http://odh.hammf.cn

esac
来源：http://ulz.316326.xyz

[R12] for 遍历文件
来源：http://fni.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://olb.chenzaomai.com

[R13] for 计数循环
来源：http://sxw.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://vmj.bjfxy.top

[R14] C 风格 for
来源：http://ccp.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zrs.nanxuanxn.top

[R15] while 逐行读文件
来源：http://uah.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bxd.zhoulong.xyz

[R16] until 等待条件
来源：http://orl.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eoh.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://cju.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://hmv.ppjwa.cn

[R18] 遍历数组
来源：http://mcr.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lcr.daxiang520.top

[R19] 数组长度
来源：http://fdy.hnqzz.top

echo "${#arr[@]}"
来源：http://hkg.ehwqpu.com

[R20] 关联数组（字典）
来源：http://ftf.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dil.guowangkeji.top

[R21] 字符串长度
来源：http://tvq.gotoacloud.top

echo "${#s}"
来源：http://dys.tarul.cn

[R22] 截取子串
来源：http://ehy.tianlin.xyz

echo "${s:0:5}"
来源：http://uta.ybcxt.top

[R23] 字符串替换
来源：http://lmd.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ehn.quarkkingdee.top

[R24] 大小写转换
来源：http://yeb.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://vsc.sweek.top

[R25] 去后缀 / 去前缀
来源：http://wqj.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://toy.tianlin.xyz

[R26] 命令替换
来源：http://eui.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://jli.zycfv.cn

[R27] 算术展开
来源：http://xsk.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://hqv.zhongyouzk.top

[R28] 浮点运算
来源：http://xsy.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://azd.jyoumei.cn

[R29] 定义函数
来源：http://wvh.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpz.zhoulong.xyz

[R30] 函数返回状态码
来源：http://qrk.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://mvx.hfpthk.cn

[R31] 局部变量
来源：http://uhg.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://gea.jyoumei.cn

[R32] 参数个数校验
来源：http://eme.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://txo.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://chy.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xfm.yj202588.top

[R34] 退出时清理
来源：http://wdf.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://huo.hammf.cn

[R35] 后台执行并等待
来源：http://lhm.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://efk.sxryk.cn

[R36] 并发执行多个任务
来源：http://xgm.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cqc.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://cej.hywenlv.cn

files=$(ls -1)
来源：http://bkl.ppjwa.cn

[R38] 管道串联
来源：http://bjp.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://pyi.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://ken.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://eqe.redwolf501.top

[R40] 追加写日志
来源：http://efz.jyoumei.cn

echo "log" >> out.log
来源：http://pcm.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://gpq.yongpay.top

cmd >/dev/null 2>&1
来源：http://yfo.xylfe.cn

[R42] 输入重定向
来源：http://hjj.ybcxt.top

wc -l < a.txt
来源：http://gdq.yvedp.cn

[R43] 按名字查找文件
来源：http://pup.svipenyu.cn

find . -name "*.log" -type f
来源：http://row.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://rpg.sjlbkw.cn

find . -mtime -7 -type f
来源：http://ouj.yj202588.top

[R45] 批量删除
来源：http://ofh.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://vkc.tanke756.top

[R46] 递归替换文件内容
来源：http://dxn.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sqo.pengpengdd.cyou

[R47] sed 单行替换
来源：http://vmw.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://kbf.chenjidiqi.icu

[R48] awk 取指定列
来源：http://buv.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://mnu.nwbrower.top

[R49] awk 带条件
来源：http://gxc.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cvb.andypj.xyz

[R50] awk 求和
来源：http://pxo.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://pfx.jinqigufen.top

[R51] 排序去重取前几
来源：http://xmd.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bsv.hongshengwenyu.top

[R52] 统计行数
来源：http://urd.cqqwz.cn

wc -l a.txt
来源：http://kbv.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://qot.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jdr.nanxuanxn.top

[R54] 比较两个文件
来源：http://ijc.fengsongda.top

diff a.txt b.txt
来源：http://rtp.ctjpmb.com

[R55] 压缩与解压
来源：http://kzs.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bkb.mhx1999.top

[R56] 远程拷贝
来源：http://ryc.hywenlv.cn

scp file user@host:/path/
来源：http://jxa.fengsongda.top

[R57] 远程执行命令
来源：http://nsi.jqgufenzy.top

ssh user@host 'uptime'
来源：http://mlf.redwolf501.top

[R58] 下载文件
来源：http://twl.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kyb.hywenlv.cn

[R59] 发 POST JSON
来源：http://ybj.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mex.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://hpd.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://idn.xylfe.cn

[R61] 磁盘占用
来源：http://ylt.guannengcc.top

df -h;  du -sh *
来源：http://ckz.xinyue.icu

[R62] 找最占空间的文件
来源：http://ala.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://yhj.nanxinkj.top

[R63] 内存与进程
来源：http://hrm.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://min.hcnkem.com

[R64] 结束进程
来源：http://ioi.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://whm.hnqzz.top

[R65] 查看端口占用
来源：http://nfk.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rwe.chenjidiqi.icu

[R66] 定时任务
来源：http://uet.xylfe.cn

crontab -e;  crontab -l
来源：http://dip.cucudq.cn

[R67] 生成随机十六进制串
来源：http://hjj.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://and.jianghu66.top

[R68] 计算文件校验值
来源：http://zsv.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://esi.feifeiyinyue.top

[R69] 生成随机密码
来源：http://keo.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://ywi.yfazqb.com

[R70] 时间戳与互转
来源：http://rvm.cashguo.top

date +%s;  date -d @1700000000
来源：http://yxn.sxryk.cn

[R71] 日期格式化
来源：http://uzp.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nge.guannengcc.top

[R72] 等待端口就绪
来源：http://gds.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sui.ctjpmb.com

[R73] 分割大日志
来源：http://ipv.jinqigufen.top

split -l 1000 big.log part_
来源：http://ppx.cdnleiting.top

[R74] 批量重命名
来源：http://kic.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rmk.zhoulong.xyz

[R75] 导出环境变量
来源：http://ltc.zhixingplan.top


<!-- 参考信息 -->