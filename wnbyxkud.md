代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dpf.andypj.xyz

[Q28] 求和与平均
来源：http://wen.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://flv.ehwqpu.com

[Q29] 最大最小值
来源：http://mxx.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mui.jlsjyb.cn

[Q30] 分组统计
来源：http://nul.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fco.ivvv.top

[Q31] 分组后过滤
来源：http://idt.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ocm.ybcxt.top

[Q32] 分组拼接字符串
来源：http://xjq.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vvi.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tak.shangyingyoupin.top

[Q33] 多列分组
来源：http://lmg.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qta.birdmap.top

[Q34] 每组取第一条
来源：http://row.smart0.xyz

SELECT * FROM (
来源：http://aer.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rpt.snrcjt.cn

) t WHERE rn = 1;
来源：http://lmz.zhaomingkeji.xyz

[Q35] 内连接
来源：http://bea.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dpj.0kj1m.cn

[Q36] 左连接
来源：http://nde.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mxi.gogol.net.cn

[Q37] 右连接
来源：http://yon.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://shd.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://erc.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jyt.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://xdd.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kno.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tts.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ekp.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vls.tanke756.top

[Q41] 多表连接
来源：http://zzt.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ygu.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://epy.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://wnv.sweek.top

[Q42] 连接条件附加过滤
来源：http://lfh.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://uyp.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rmi.jqgfzy.top

[Q43] 标量子查询
来源：http://bxm.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://duz.yuxming.cn

[Q44] IN 子查询
来源：http://yoe.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xsx.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://cnz.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kbv.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cst.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpg.chenzaomai.com

[Q47] 与平均值比较
来源：http://dtf.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ccy.yj202588.top

[Q48] CTE 公用表表达式
来源：http://lrm.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gwb.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://ddp.chenjidiqi.icu

[Q49] 更新单行
来源：http://ova.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aej.tianlin.xyz

[Q50] 批量更新
来源：http://rkr.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nzy.zhongyouzk.top

[Q51] 用子查询更新
来源：http://pek.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ldu.redwolf501.top

[Q52] 删除指定行
来源：http://lih.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://zwi.zdbjq.cn

[Q53] 按条件删除
来源：http://pkr.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fxl.jiagoushi.top

[Q54] 清空表
来源：http://lsj.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://eqa.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://hlz.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nhr.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://glf.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yab.guannengcc.top

[Q57] 行号
来源：http://oaz.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ezx.havefunace.top

[Q58] 累计求和
来源：http://art.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://urd.hnqzz.top

[Q59] 分组内累计
来源：http://iva.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kok.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://rsl.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xhy.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://frj.iojbl.cn

[Q61] 移动平均
来源：http://yap.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://crc.fzhhl.top

[Q62] 分组占比
来源：http://bld.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lor.zhoulong.xyz

[Q63] 开启事务
来源：http://qly.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rzc.cdnleiting.top

[Q64] 提交事务
来源：http://urq.nanxuanxn.top

COMMIT;
来源：http://nhz.tianlin.xyz

[Q65] 回滚事务
来源：http://ckr.epnwcf.com

ROLLBACK;
来源：http://jtk.tanke756.top

[Q66] 行锁查询
来源：http://ylv.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tkq.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://qif.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mvk.zhiwuduotai.top

[Q68] 保存点
来源：http://knt.vqdsnc.cn

SAVEPOINT sp1;
来源：http://jpm.9152youxi.cn

ROLLBACK TO sp1;
来源：http://xpw.52xcode.cn

[Q69] 查看执行计划
来源：http://zsl.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://auv.cdnleiting.top

[Q70] 更新统计信息
来源：http://fzl.fengsongda.top

ANALYZE TABLE users;
来源：http://tvk.yanxiufei.cn

[Q71] 查看建表语句
来源：http://ket.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rlw.yj202588.top

[Q72] 查看索引
来源：http://nyd.jianghu66.top

SHOW INDEX FROM users;
来源：http://ozu.yuxming.cn

[Q73] 查看表状态
来源：http://uol.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://idu.vqdsnc.cn

[Q74] 强制使用索引
来源：http://niz.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://poq.yuxming.cn

[Q75] 日期格式化
来源：http://igw.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://giu.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dsa.havefunace.top

[Q76] 按天统计
来源：http://wyw.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fme.jqgufenzy.top

[Q77] 时间加减
来源：http://hoi.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xpw.fzhhl.top

[Q78] 当前时间
来源：http://miy.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cpf.kuanghao11.cn

[Q79] 字符串拼接
来源：http://ckd.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wci.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://qqh.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jli.yfazqb.com

[Q81] 字符串替换
来源：http://mjx.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://slc.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://wrh.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://poa.haohaochexian.top

[Q83] 大小写转换
来源：http://gat.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gff.zdbjq.cn

[Q84] 去除首尾空格
来源：http://nia.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://gyr.daria6918.cn

[Q85] 数值取整
来源：http://gti.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vso.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://gtn.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://itc.hnqzz.top

[Q87] JSON 字段做条件
来源：http://tgq.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mez.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://kcm.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gce.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ndh.fzhhl.top

[Q89] 判断表是否存在
来源：http://cuk.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ffc.jlsjyb.cn

[Q90] 生成序号列
来源：http://fxd.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fdq.0kj1m.cn

================================================================================
来源：http://mwf.yj202588.top

R. Bash 专题
来源：http://ovo.tian-w.cn

================================================================================
来源：http://ojc.redwolf501.top

[R01] shebang 与严格模式
来源：http://djc.ppjwa.cn

#!/usr/bin/env bash
来源：http://fui.xinyue.icu

set -euo pipefail
来源：http://gda.sxryk.cn

[R02] 变量赋值与使用
来源：http://zpt.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://cat.feifeiyinyue.top

[R03] 只读变量
来源：http://fao.ybcxt.top

readonly PI=3.14
来源：http://enj.shanyushiyangtech.top

[R04] 位置参数
来源：http://mfz.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vxn.52xcode.cn

[R05] 参数默认值
来源：http://wwu.fktsv.cn

name="${1:-default}"
来源：http://yho.hfpthk.cn

[R06] 判断命令是否存在
来源：http://wed.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zpv.sjlbkw.cn

[R07] if 判断文件
来源：http://mbz.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yux.pengpengdd.cyou

[R08] 数值比较
来源：http://vuo.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tel.zdbjq.cn

[R09] 字符串比较
来源：http://gqi.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mfm.wangshuangyany.cn

[R10] 正则匹配
来源：http://jlf.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gwh.cqqwz.cn

[R11] case 多分支
来源：http://gyl.haohaochexian.top

case "$1" in
来源：http://rwa.zdqjudy.top

start) echo "启动" ;;
来源：http://rjl.cheryme.top

stop)  echo "停止" ;;
来源：http://xvh.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://cop.hnqzz.top

esac
来源：http://bvx.mhx1999.top

[R12] for 遍历文件
来源：http://yky.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://acz.bbcook.cn

[R13] for 计数循环
来源：http://wyf.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://dfl.meibo888.top

[R14] C 风格 for
来源：http://fks.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dkw.snrcjt.cn

[R15] while 逐行读文件
来源：http://flj.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vwy.fzhhl.top

[R16] until 等待条件
来源：http://flb.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qqc.yangfankeji.com

[R17] 数组定义与取值
来源：http://arq.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://twn.aizwys.cn

[R18] 遍历数组
来源：http://gor.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wzv.yj20258.top

[R19] 数组长度
来源：http://dmd.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://qqg.iojbl.cn

[R20] 关联数组（字典）
来源：http://nmd.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://adm.feifeiyinyue.top

[R21] 字符串长度
来源：http://cbw.uphjek.com

echo "${#s}"
来源：http://qeu.yongpay.top

[R22] 截取子串
来源：http://ilx.havefunace.top

echo "${s:0:5}"
来源：http://kae.feifeiyinyue.top

[R23] 字符串替换
来源：http://vmc.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pdi.shangyingyoupin.top

[R24] 大小写转换
来源：http://ghm.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://dys.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://rmm.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://uyu.zhijiandao.cn

[R26] 命令替换
来源：http://ngd.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://ueh.jinghuilouyu.cn

[R27] 算术展开
来源：http://eok.gzhubu.top

echo $((1 + 2 * 3))
来源：http://bkg.guannengcc.top

[R28] 浮点运算
来源：http://qqq.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://fag.jqgufenzy.top

[R29] 定义函数
来源：http://pxx.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qpj.jqgfzy.top

[R30] 函数返回状态码
来源：http://lbf.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://yxm.vqdsnc.cn

[R31] 局部变量
来源：http://jct.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://vdm.havefunace.top

[R32] 参数个数校验
来源：http://wkl.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wci.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://ivb.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oxe.bbcook.cn

[R34] 退出时清理
来源：http://rjl.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://kpq.xuanzx.com

[R35] 后台执行并等待
来源：http://dtp.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gqs.zhixingplan.top

[R36] 并发执行多个任务
来源：http://cgq.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qsl.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://pnz.ehwqpu.com

files=$(ls -1)
来源：http://xvu.zhongyouzk.top

[R38] 管道串联
来源：http://ltq.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://yzw.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://dkh.yj202588.top

cmd > out.log 2>&1
来源：http://ihj.fanxiaobao.xyz

[R40] 追加写日志
来源：http://sdm.daria6918.cn

echo "log" >> out.log
来源：http://jpn.xuetiantiany.cn

[R41] 丢弃输出
来源：http://isl.cucudq.cn

cmd >/dev/null 2>&1
来源：http://dpk.zhiwuduotai.top

[R42] 输入重定向
来源：http://emi.ywan-chungtsiang.top

wc -l < a.txt
来源：http://bfn.nanxinkj.top

[R43] 按名字查找文件
来源：http://mun.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://oxj.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://fwp.yueranfly.top

find . -mtime -7 -type f
来源：http://zfc.gaohongyu789.top

[R45] 批量删除
来源：http://hub.jianghu66.top

find . -name "*.tmp" -delete
来源：http://gop.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://cya.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jbf.snrcjt.cn

[R47] sed 单行替换
来源：http://gib.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://ush.fengsongda.top

[R48] awk 取指定列
来源：http://krt.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://ujb.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://vum.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avl.uphjek.com

[R50] awk 求和
来源：http://oxu.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ikd.jqgufenzy.top

[R51] 排序去重取前几
来源：http://lug.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ess.xuanzx.com

[R52] 统计行数
来源：http://tki.quarkkingdee.top

wc -l a.txt
来源：http://tds.yonumen.top

[R53] 查看文件头与实时尾
来源：http://ofj.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xpk.fktsv.cn

[R54] 比较两个文件
来源：http://bxe.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://lll.zhongyouzk.top

[R55] 压缩与解压
来源：http://pzj.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vnb.hesvh.cn

[R56] 远程拷贝
来源：http://kqw.iojbl.cn

scp file user@host:/path/
来源：http://pir.zycfv.cn

[R57] 远程执行命令
来源：http://hza.aibaodan.cn

ssh user@host 'uptime'
来源：http://ekz.uphjek.com

[R58] 下载文件
来源：http://kya.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ond.jyoumei.cn

[R59] 发 POST JSON
来源：http://mmb.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qsm.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://ndo.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yex.guannengcc.top

[R61] 磁盘占用
来源：http://nsi.tian-w.cn

df -h;  du -sh *
来源：http://fwn.yvedp.cn

[R62] 找最占空间的文件
来源：http://pyq.tarul.cn

du -ah . | sort -rh | head -10
来源：http://eij.bjfxy.top

[R63] 内存与进程
来源：http://jco.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://asl.cheryme.top

[R64] 结束进程
来源：http://mqn.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://lyj.gogol.net.cn

[R65] 查看端口占用
来源：http://brl.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hea.yuanzhike.top

[R66] 定时任务
来源：http://tbs.xuanzx.com

crontab -e;  crontab -l
来源：http://kts.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://hxu.sweek.top

openssl rand -hex 16
来源：http://ogo.vehdjk.com

[R68] 计算文件校验值
来源：http://hak.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://axn.jqgufenzy.top

[R69] 生成随机密码
来源：http://ibt.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://vie.chenlongwang.top

[R70] 时间戳与互转
来源：http://mds.cucudq.cn

date +%s;  date -d @1700000000
来源：http://eof.nanxinkj.top

[R71] 日期格式化
来源：http://ebh.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://azs.zhengqikj.top

[R72] 等待端口就绪
来源：http://vtb.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vlb.cqqwz.cn

[R73] 分割大日志
来源：http://lxb.shuidangran.top

split -l 1000 big.log part_
来源：http://eey.birdmap.top

[R74] 批量重命名
来源：http://qgs.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uxt.zdbjq.cn

[R75] 导出环境变量
来源：http://uby.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://nsn.shzxlz.cn

[R76] 使用临时文件
来源：http://tns.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cga.fktsv.cn

[R77] 读取用户输入
来源：http://kol.0kj1m.cn


<!-- 参考信息 -->