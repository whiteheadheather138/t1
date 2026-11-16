代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://axd.ywan-chungtsiang.top

[Q22] 排序
来源：http://onb.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://omz.ppjwa.cn

[Q23] 分页
来源：http://rme.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jfz.jinqigufen.top

[Q24] 去重
来源：http://ixd.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://qmf.meibo888.top

[Q25] 只取前 N 条
来源：http://qhk.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hda.yj202588.top

[Q26] 计数
来源：http://ldh.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://xtc.hywenlv.cn

[Q27] 条件计数
来源：http://zmc.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qdc.jinqigfzy.top

[Q28] 求和与平均
来源：http://yau.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fld.zhijiandao.cn

[Q29] 最大最小值
来源：http://dpz.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://luf.cucudq.cn

[Q30] 分组统计
来源：http://eob.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://onu.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://bhv.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jnh.yueranfly.top

[Q32] 分组拼接字符串
来源：http://mxk.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pda.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://doz.gogol.net.cn

[Q33] 多列分组
来源：http://cnf.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zpi.snrcjt.cn

[Q34] 每组取第一条
来源：http://tnu.chenjidiqi.icu

SELECT * FROM (
来源：http://qkm.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://buw.nwbrower.top

) t WHERE rn = 1;
来源：http://lae.fehbvm.com

[Q35] 内连接
来源：http://fqs.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eld.pengpengdd.cyou

[Q36] 左连接
来源：http://xwo.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rzo.cqqwz.cn

[Q37] 右连接
来源：http://ndw.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gha.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://kau.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aso.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://ycy.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://szw.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mmz.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://afs.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tdj.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://mxl.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://lbm.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://ttg.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://rrs.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://mvc.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://mdd.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hkh.ivvv.top

[Q43] 标量子查询
来源：http://gua.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kbp.yueranfly.top

[Q44] IN 子查询
来源：http://yip.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kzp.316326.xyz

[Q45] EXISTS 判断存在
来源：http://ozf.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hlf.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://dbb.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exv.dianchejie.cn

[Q47] 与平均值比较
来源：http://kat.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lmy.tanke756.top

[Q48] CTE 公用表表达式
来源：http://lmx.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zyl.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://lqc.xuanzx.com

[Q49] 更新单行
来源：http://zkk.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hop.nanxinkj.top

[Q50] 批量更新
来源：http://mxa.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qid.shuidangran.top

[Q51] 用子查询更新
来源：http://fdt.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jjp.smart0.xyz

[Q52] 删除指定行
来源：http://kvy.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://nqk.snrcjt.cn

[Q53] 按条件删除
来源：http://ogq.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mzj.hesvh.cn

[Q54] 清空表
来源：http://ejp.fehbvm.com

TRUNCATE TABLE logs;
来源：http://uwh.uphjek.com

[Q55] 排名（并列占位）
来源：http://vzc.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bfv.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://hye.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nvo.316326.xyz

[Q57] 行号
来源：http://cpr.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ptk.bjfxy.top

[Q58] 累计求和
来源：http://vap.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gtx.redwolf501.top

[Q59] 分组内累计
来源：http://bbz.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ubz.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://wrz.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mmv.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eil.yonumen.top

[Q61] 移动平均
来源：http://qfg.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pzk.cqqwz.cn

[Q62] 分组占比
来源：http://xen.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://abv.redwolf501.top

[Q63] 开启事务
来源：http://nsl.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://grm.sweek.top

[Q64] 提交事务
来源：http://rjq.vqdsnc.cn

COMMIT;
来源：http://toy.hnxiangtu.top

[Q65] 回滚事务
来源：http://awm.havefunace.top

ROLLBACK;
来源：http://hit.yueranfly.top

[Q66] 行锁查询
来源：http://qus.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mcm.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://hls.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xdq.hfpthk.cn

[Q68] 保存点
来源：http://wui.pycfn.com

SAVEPOINT sp1;
来源：http://jwm.yj20258.top

ROLLBACK TO sp1;
来源：http://wfl.zhongyouzk.top

[Q69] 查看执行计划
来源：http://slv.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lcn.aizwys.cn

[Q70] 更新统计信息
来源：http://hyv.zdbjq.cn

ANALYZE TABLE users;
来源：http://eue.hnxiangtu.top

[Q71] 查看建表语句
来源：http://ctl.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pxk.quarkkingdee.top

[Q72] 查看索引
来源：http://baj.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://rnr.guannengcc.top

[Q73] 查看表状态
来源：http://lxo.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tlt.smart0.xyz

[Q74] 强制使用索引
来源：http://gqj.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xug.zhengqikj.top

[Q75] 日期格式化
来源：http://cjr.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wtf.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lyj.yj20258.top

[Q76] 按天统计
来源：http://hdp.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hkr.fengsongda.top

[Q77] 时间加减
来源：http://abx.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uqb.hnxiangtu.top

[Q78] 当前时间
来源：http://arf.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wib.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://cok.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sxa.zdbjq.cn

[Q80] 字符串截取
来源：http://zwa.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bmw.guannengcc.top

[Q81] 字符串替换
来源：http://aml.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vwa.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://ibe.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kvl.nanxinkj.top

[Q83] 大小写转换
来源：http://boa.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fpc.nwbrower.top

[Q84] 去除首尾空格
来源：http://fno.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://amd.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://qaw.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwx.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://kuc.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wgy.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://lwp.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ocv.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://hkm.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uac.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://obt.xylfe.cn

[Q89] 判断表是否存在
来源：http://bbo.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kos.hywenlv.cn

[Q90] 生成序号列
来源：http://awh.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sww.jinqigfzy.top

================================================================================
来源：http://qce.hysaishi.cn

R. Bash 专题
来源：http://rfp.yuanzhike.top

================================================================================
来源：http://qvg.cqqwz.cn

[R01] shebang 与严格模式
来源：http://dqu.zhijiandao.cn

#!/usr/bin/env bash
来源：http://hok.zhijiandao.cn

set -euo pipefail
来源：http://obn.tianlin.xyz

[R02] 变量赋值与使用
来源：http://xuk.zdqjudy.top

name="Tom"; echo "$name"
来源：http://tie.zhijiandao.cn

[R03] 只读变量
来源：http://tfh.ybcxt.top

readonly PI=3.14
来源：http://qzz.hongshengwenyu.top

[R04] 位置参数
来源：http://xvj.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://omt.hammf.cn

[R05] 参数默认值
来源：http://wyt.sysykeji.top

name="${1:-default}"
来源：http://nzs.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://snl.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ybo.zycfv.cn

[R07] if 判断文件
来源：http://tld.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mmv.zhengqikj.top

[R08] 数值比较
来源：http://xzs.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hrb.vqdsnc.cn

[R09] 字符串比较
来源：http://ids.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cbj.fzhhl.top

[R10] 正则匹配
来源：http://jsv.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mnh.quarkkingdee.top

[R11] case 多分支
来源：http://jhp.xuetiantiany.cn

case "$1" in
来源：http://knx.nwbrower.top

start) echo "启动" ;;
来源：http://fzk.jinqigufen.top

stop)  echo "停止" ;;
来源：http://ykh.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://cre.sxryk.cn

esac
来源：http://pta.kuanghao11.cn

[R12] for 遍历文件
来源：http://rnb.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://thi.fehbvm.com

[R13] for 计数循环
来源：http://tso.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://aci.cdnleiting.top

[R14] C 风格 for
来源：http://tsn.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cac.birdmap.top

[R15] while 逐行读文件
来源：http://lsh.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dyd.9152youxi.cn

[R16] until 等待条件
来源：http://yde.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ayn.meibo888.top

[R17] 数组定义与取值
来源：http://prh.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://oju.guannengcc.top

[R18] 遍历数组
来源：http://zmi.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukk.tarul.cn

[R19] 数组长度
来源：http://nvp.iojbl.cn

echo "${#arr[@]}"
来源：http://afs.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://oaa.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bwf.yangfankeji.com

[R21] 字符串长度
来源：http://mck.zhoulong.xyz

echo "${#s}"
来源：http://mru.pycfn.com

[R22] 截取子串
来源：http://jyw.quarkkingdee.top

echo "${s:0:5}"
来源：http://bbu.cheryme.top

[R23] 字符串替换
来源：http://fnu.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pab.zycfv.cn

[R24] 大小写转换
来源：http://zfj.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://zem.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://uuh.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xzi.yangfankeji.com

[R26] 命令替换
来源：http://wzw.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://jdf.cqqwz.cn

[R27] 算术展开
来源：http://jjp.jianghu66.top

echo $((1 + 2 * 3))
来源：http://jzc.chenlongwang.top

[R28] 浮点运算
来源：http://lzy.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://khr.yanxiufei.cn

[R29] 定义函数
来源：http://kin.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://azd.nanxinkj.top

[R30] 函数返回状态码
来源：http://qnk.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://fem.jinghuilouyu.cn

[R31] 局部变量
来源：http://rgp.sweek.top

f() { local x=1; echo "$x"; }
来源：http://qzd.zhoulong.xyz

[R32] 参数个数校验
来源：http://rxy.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tme.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://mkh.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tmn.sxryk.cn

[R34] 退出时清理
来源：http://ryo.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://qek.daxiang520.top

[R35] 后台执行并等待
来源：http://hwl.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://azd.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://rvh.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://skv.iojbl.cn

[R37] 把输出赋给变量
来源：http://lam.aizwys.cn

files=$(ls -1)
来源：http://nir.xinyue.icu

[R38] 管道串联
来源：http://ygh.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://iqx.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://ktl.meibo888.top

cmd > out.log 2>&1
来源：http://lxm.redwolf501.top

[R40] 追加写日志
来源：http://uvd.tanke756.top

echo "log" >> out.log
来源：http://zav.hywenlv.cn

[R41] 丢弃输出
来源：http://yor.hammf.cn

cmd >/dev/null 2>&1
来源：http://tcg.gzhubu.top

[R42] 输入重定向
来源：http://oig.zycfv.cn

wc -l < a.txt
来源：http://wro.yonumen.top

[R43] 按名字查找文件
来源：http://tbm.ybcxt.top

find . -name "*.log" -type f
来源：http://aew.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://gtt.andypj.xyz

find . -mtime -7 -type f
来源：http://jfx.tarul.cn

[R45] 批量删除
来源：http://swx.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://kek.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://exg.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipw.ybcxt.top

[R47] sed 单行替换
来源：http://yhv.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://phy.shzxlz.cn

[R48] awk 取指定列
来源：http://dle.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://icf.epnwcf.com

[R49] awk 带条件
来源：http://dwk.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zqj.shanyushiyangtech.top

[R50] awk 求和
来源：http://yfd.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hmw.tanke756.top

[R51] 排序去重取前几
来源：http://lmy.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jpr.jiagoushi.top

[R52] 统计行数
来源：http://khd.yuxming.cn

wc -l a.txt
来源：http://bjb.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://xgs.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://skg.havefunace.top

[R54] 比较两个文件
来源：http://ufv.fanxiaobao.xyz

diff a.txt b.txt
来源：http://zoc.yj202588.top

[R55] 压缩与解压
来源：http://ser.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fke.yongpay.top

[R56] 远程拷贝
来源：http://cff.andypj.xyz

scp file user@host:/path/
来源：http://zsq.hnqzz.top

[R57] 远程执行命令
来源：http://djs.nanxinkj.top

ssh user@host 'uptime'
来源：http://jxe.uphjek.com

[R58] 下载文件
来源：http://yuy.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uvn.hysaishi.cn

[R59] 发 POST JSON
来源：http://bpd.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ijn.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://omk.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fby.ctjpmb.com

[R61] 磁盘占用
来源：http://twa.redwolf501.top

df -h;  du -sh *
来源：http://uvv.gogol.net.cn

[R62] 找最占空间的文件
来源：http://pmu.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://dsx.guannengcc.top

[R63] 内存与进程
来源：http://ubv.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://foq.ybcxt.top

[R64] 结束进程
来源：http://bug.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://wpy.ctjpmb.com

[R65] 查看端口占用
来源：http://xzt.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ynd.epnwcf.com

[R66] 定时任务
来源：http://smm.52xcode.cn

crontab -e;  crontab -l
来源：http://jrg.jianghu66.top

[R67] 生成随机十六进制串
来源：http://flt.sysykeji.top

openssl rand -hex 16
来源：http://dwy.ehwqpu.com

[R68] 计算文件校验值
来源：http://ynm.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://cpl.fengsongda.top

[R69] 生成随机密码
来源：http://rwv.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://lzo.fzhhl.top

[R70] 时间戳与互转
来源：http://ghn.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://sud.shanyushiyangtech.top

[R71] 日期格式化
来源：http://yuy.aizwys.cn


<!-- 参考信息 -->