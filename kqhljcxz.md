代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mep.yuxming.cn

[Q28] 求和与平均
来源：http://rxn.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sef.feifeiyinyue.top

[Q29] 最大最小值
来源：http://pyi.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ind.daxiang520.top

[Q30] 分组统计
来源：http://uus.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dqa.zhongyouzk.top

[Q31] 分组后过滤
来源：http://gxp.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lgs.aizwys.cn

[Q32] 分组拼接字符串
来源：http://txz.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hfr.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vdp.ydzc1.top

[Q33] 多列分组
来源：http://fsl.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rwo.0kj1m.cn

[Q34] 每组取第一条
来源：http://ixm.sjlbkw.cn

SELECT * FROM (
来源：http://cpv.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hcl.zdbjq.cn

) t WHERE rn = 1;
来源：http://iid.zhixingplan.top

[Q35] 内连接
来源：http://ctc.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aaq.tianlin.xyz

[Q36] 左连接
来源：http://tvp.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zjc.fktsv.cn

[Q37] 右连接
来源：http://erp.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ndj.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://xea.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://otr.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://wlj.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xpr.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qvs.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pnm.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fow.yangfankeji.com

[Q41] 多表连接
来源：http://gzq.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nux.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://yde.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://tsu.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://sbi.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://pdi.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wdf.gotoacloud.top

[Q43] 标量子查询
来源：http://ymz.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tfb.jinqigfzy.top

[Q44] IN 子查询
来源：http://owi.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dmm.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://cjd.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fmz.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://yyd.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ihf.zycfv.cn

[Q47] 与平均值比较
来源：http://ofs.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cbs.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://ugi.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uvp.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://fbu.sufxvd.cn

[Q49] 更新单行
来源：http://bip.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://isv.cqqwz.cn

[Q50] 批量更新
来源：http://rou.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mzj.nwbrower.top

[Q51] 用子查询更新
来源：http://lzg.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zmq.sysykeji.top

[Q52] 删除指定行
来源：http://mnu.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://dac.cashguo.top

[Q53] 按条件删除
来源：http://dst.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vjy.hammf.cn

[Q54] 清空表
来源：http://odp.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://mjs.gzhubu.top

[Q55] 排名（并列占位）
来源：http://dxh.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ppj.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://njn.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jca.yj20258888.top

[Q57] 行号
来源：http://beo.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bkq.ppjwa.cn

[Q58] 累计求和
来源：http://iii.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wvb.ybcxt.top

[Q59] 分组内累计
来源：http://nhr.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fzx.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://uge.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nkb.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tek.bjfxy.top

[Q61] 移动平均
来源：http://dze.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://suu.xinyue.icu

[Q62] 分组占比
来源：http://bxb.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dvn.dashuyun.cn

[Q63] 开启事务
来源：http://elp.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sdh.zhijiandao.cn

[Q64] 提交事务
来源：http://onr.havefunace.top

COMMIT;
来源：http://quc.iojbl.cn

[Q65] 回滚事务
来源：http://nni.tian-w.cn

ROLLBACK;
来源：http://qea.gzhubu.top

[Q66] 行锁查询
来源：http://mlz.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rrk.gotoacloud.top

[Q67] 设置隔离级别
来源：http://ffy.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pki.iojbl.cn

[Q68] 保存点
来源：http://wbd.xuanzx.com

SAVEPOINT sp1;
来源：http://qet.hammf.cn

ROLLBACK TO sp1;
来源：http://iim.yonumen.top

[Q69] 查看执行计划
来源：http://ehu.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ylu.yonumen.top

[Q70] 更新统计信息
来源：http://twa.yueranfly.top

ANALYZE TABLE users;
来源：http://gwb.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://ouw.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mhf.cdnleiting.top

[Q72] 查看索引
来源：http://mba.cqqwz.cn

SHOW INDEX FROM users;
来源：http://itm.nanxuanxn.top

[Q73] 查看表状态
来源：http://djr.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nhw.snrcjt.cn

[Q74] 强制使用索引
来源：http://vmi.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wgo.gotoacloud.top

[Q75] 日期格式化
来源：http://wce.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://chh.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jzx.redwolf501.top

[Q76] 按天统计
来源：http://xub.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eol.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://squ.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ulm.bbcook.cn

[Q78] 当前时间
来源：http://lvq.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yfs.nanxinkj.top

[Q79] 字符串拼接
来源：http://kiz.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oxn.vqdsnc.cn

[Q80] 字符串截取
来源：http://zvd.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ydc.jianghu66.top

[Q81] 字符串替换
来源：http://usa.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xav.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://sdq.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://amx.mhx1999.top

[Q83] 大小写转换
来源：http://pnx.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://npq.yangfankeji.com

[Q84] 去除首尾空格
来源：http://tvo.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://wcr.quarkkingdee.top

[Q85] 数值取整
来源：http://yep.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qdd.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://wlx.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://csx.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://rgf.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vjw.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://zfa.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ttp.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nef.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://uqu.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ajr.aibaodan.cn

[Q90] 生成序号列
来源：http://ueg.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qpp.cdnleiting.top

================================================================================
来源：http://whe.yuanzhike.top

R. Bash 专题
来源：http://efn.xingfuxueyuan.xyz

================================================================================
来源：http://rti.ppjwa.cn

[R01] shebang 与严格模式
来源：http://rax.vqdsnc.cn

#!/usr/bin/env bash
来源：http://gpo.jqgfzy.top

set -euo pipefail
来源：http://yac.zdqjudy.top

[R02] 变量赋值与使用
来源：http://zwg.fzhhl.top

name="Tom"; echo "$name"
来源：http://azr.yongpay.top

[R03] 只读变量
来源：http://aks.mhx1999.top

readonly PI=3.14
来源：http://tmj.kuanghao11.cn

[R04] 位置参数
来源：http://mva.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hlv.gotoacloud.top

[R05] 参数默认值
来源：http://sjz.kuanghao11.cn

name="${1:-default}"
来源：http://sve.daxiang520.top

[R06] 判断命令是否存在
来源：http://dzv.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bgh.sufxvd.cn

[R07] if 判断文件
来源：http://ygt.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zxj.yuanzhike.top

[R08] 数值比较
来源：http://nnp.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://mof.aibaodan.cn

[R09] 字符串比较
来源：http://cpq.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hzj.redwolf501.top

[R10] 正则匹配
来源：http://ost.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cws.yj20258.top

[R11] case 多分支
来源：http://fxq.chenzaomai.com

case "$1" in
来源：http://kdq.havefunace.top

start) echo "启动" ;;
来源：http://qkr.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://zon.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://unw.hnqzz.top

esac
来源：http://czz.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://apt.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://uya.chenzaomai.com

[R13] for 计数循环
来源：http://vas.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://thc.zhongyouzk.top

[R14] C 风格 for
来源：http://kgj.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iho.daxiang520.top

[R15] while 逐行读文件
来源：http://few.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://khq.quarkkingdee.top

[R16] until 等待条件
来源：http://kkf.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://awy.xuanzx.com

[R17] 数组定义与取值
来源：http://rhu.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://qth.shuidangran.top

[R18] 遍历数组
来源：http://bgu.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tcm.yfazqb.com

[R19] 数组长度
来源：http://ahb.nwbrower.top

echo "${#arr[@]}"
来源：http://tca.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://oyv.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mzo.sjlbkw.cn

[R21] 字符串长度
来源：http://mzw.yuxming.cn

echo "${#s}"
来源：http://bot.andypj.xyz

[R22] 截取子串
来源：http://btv.gzhubu.top

echo "${s:0:5}"
来源：http://mcm.ctjpmb.com

[R23] 字符串替换
来源：http://qub.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yie.jinqigufen.top

[R24] 大小写转换
来源：http://res.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fxa.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://lwn.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nwi.zhaomingkeji.xyz

[R26] 命令替换
来源：http://aln.meibo888.top

now=$(date +%F); echo "$now"
来源：http://gqa.yongpay.top

[R27] 算术展开
来源：http://lin.fengsongda.top

echo $((1 + 2 * 3))
来源：http://kaw.mhx1999.top

[R28] 浮点运算
来源：http://dkp.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://tri.nanxinkj.top

[R29] 定义函数
来源：http://ikd.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gra.yj20258.top

[R30] 函数返回状态码
来源：http://euk.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://rfw.shzxlz.cn

[R31] 局部变量
来源：http://fhf.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://kox.cucudq.cn

[R32] 参数个数校验
来源：http://rov.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dft.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://okj.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cjp.fengsongda.top

[R34] 退出时清理
来源：http://vqk.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://rmu.iojbl.cn

[R35] 后台执行并等待
来源：http://nzd.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://usq.fengsongda.top

[R36] 并发执行多个任务
来源：http://ygi.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ush.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://npu.chenlongwang.top

files=$(ls -1)
来源：http://bmu.ywan-chungtsiang.top

[R38] 管道串联
来源：http://gwh.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://kva.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://req.yuanzhike.top

cmd > out.log 2>&1
来源：http://snw.yuanzhike.top

[R40] 追加写日志
来源：http://zsr.tarul.cn

echo "log" >> out.log
来源：http://jvx.gaohongyu789.top

[R41] 丢弃输出
来源：http://kzh.xuanzx.com

cmd >/dev/null 2>&1
来源：http://ahp.fktsv.cn

[R42] 输入重定向
来源：http://uob.pycfn.com

wc -l < a.txt
来源：http://zdr.hcnkem.com

[R43] 按名字查找文件
来源：http://lla.quarkkingdee.top

find . -name "*.log" -type f
来源：http://umt.tarul.cn

[R44] 按修改时间查找
来源：http://qua.52xcode.cn

find . -mtime -7 -type f
来源：http://tsi.daria6918.cn

[R45] 批量删除
来源：http://wpc.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://mch.0kj1m.cn

[R46] 递归替换文件内容
来源：http://nrd.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nkk.meibo888.top

[R47] sed 单行替换
来源：http://bjc.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://azu.aizwys.cn

[R48] awk 取指定列
来源：http://ojw.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://xuh.quarkkingdee.top

[R49] awk 带条件
来源：http://wuk.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uev.tianlin.xyz

[R50] awk 求和
来源：http://uhh.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aqc.ppjwa.cn

[R51] 排序去重取前几
来源：http://nmp.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uaz.birdmap.top

[R52] 统计行数
来源：http://hnz.shanyushiyangtech.top

wc -l a.txt
来源：http://lxj.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://lud.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fns.yanxiufei.cn

[R54] 比较两个文件
来源：http://mlr.ppjwa.cn

diff a.txt b.txt
来源：http://zdw.hnxiangtu.top

[R55] 压缩与解压
来源：http://euc.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sdd.cashguo.top

[R56] 远程拷贝
来源：http://hli.zhijiandao.cn

scp file user@host:/path/
来源：http://jyf.xuetiantiany.cn

[R57] 远程执行命令
来源：http://kcr.zhixingplan.top

ssh user@host 'uptime'
来源：http://fdu.gogol.net.cn

[R58] 下载文件
来源：http://wfb.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oox.9152youxi.cn

[R59] 发 POST JSON
来源：http://gwz.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vcu.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://izm.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pno.sufxvd.cn

[R61] 磁盘占用
来源：http://sjp.jinghuilouyu.cn

df -h;  du -sh *
来源：http://wxq.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://vie.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://uth.sjlbkw.cn

[R63] 内存与进程
来源：http://hnj.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://mhq.epnwcf.com

[R64] 结束进程
来源：http://nlt.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://clu.aibaodan.cn

[R65] 查看端口占用
来源：http://nni.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://umm.guowangkeji.top

[R66] 定时任务
来源：http://xaw.ehwqpu.com

crontab -e;  crontab -l
来源：http://pjt.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://tgq.cashguo.top

openssl rand -hex 16
来源：http://qru.zhixingplan.top

[R68] 计算文件校验值
来源：http://gct.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://kcw.cashguo.top

[R69] 生成随机密码
来源：http://rhi.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://pyb.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://did.tarul.cn

date +%s;  date -d @1700000000
来源：http://rwv.jinqigufen.top

[R71] 日期格式化
来源：http://xao.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rhu.shuidangran.top

[R72] 等待端口就绪
来源：http://akf.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bry.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://mot.guowangkeji.top

split -l 1000 big.log part_
来源：http://swe.ydjk.org.cn

[R74] 批量重命名
来源：http://bct.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cjb.cqqwz.cn

[R75] 导出环境变量
来源：http://csf.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://ytr.hnqzz.top

[R76] 使用临时文件
来源：http://zou.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lqs.guowangkeji.top

[R77] 读取用户输入
来源：http://ufr.cheryme.top


<!-- 参考信息 -->