代发 wailian999

[Q33] 多列分组
来源：http://nfw.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbe.zhixingplan.top

[Q34] 每组取第一条
来源：http://vub.yvedp.cn

SELECT * FROM (
来源：http://yph.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bqz.guowangkeji.top

) t WHERE rn = 1;
来源：http://dob.jianghu66.top

[Q35] 内连接
来源：http://dqj.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fdf.epnwcf.com

[Q36] 左连接
来源：http://udm.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mzd.chenlongwang.top

[Q37] 右连接
来源：http://lpq.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uwr.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://huz.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://agu.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://ibr.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hpp.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gqp.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://lho.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lfm.andypj.xyz

[Q41] 多表连接
来源：http://fll.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://man.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://snt.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://brc.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://xek.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://jqj.sjlbkw.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ync.yuxming.cn

[Q43] 标量子查询
来源：http://ior.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://clc.fengsongda.top

[Q44] IN 子查询
来源：http://exz.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vwg.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://qyw.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkj.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://wtz.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdh.yvedp.cn

[Q47] 与平均值比较
来源：http://ukg.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rrc.cashguo.top

[Q48] CTE 公用表表达式
来源：http://pvr.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zlg.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://lxc.yueranfly.top

[Q49] 更新单行
来源：http://kmp.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oea.pycfn.com

[Q50] 批量更新
来源：http://zlh.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tug.fengsongda.top

[Q51] 用子查询更新
来源：http://eqh.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ypz.gogol.net.cn

[Q52] 删除指定行
来源：http://hez.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://ekv.xinyue.icu

[Q53] 按条件删除
来源：http://iiz.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://buo.c1oappe.top

[Q54] 清空表
来源：http://xta.tanke756.top

TRUNCATE TABLE logs;
来源：http://acc.daxiang520.top

[Q55] 排名（并列占位）
来源：http://wse.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fcb.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://ahz.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pic.xylfe.cn

[Q57] 行号
来源：http://zxh.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dwa.0kj1m.cn

[Q58] 累计求和
来源：http://mhq.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://miu.gzhubu.top

[Q59] 分组内累计
来源：http://qni.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://moo.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://frr.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pxj.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zom.haohaochexian.top

[Q61] 移动平均
来源：http://vzy.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pyk.zhengqikj.top

[Q62] 分组占比
来源：http://dva.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ffc.shzxlz.cn

[Q63] 开启事务
来源：http://syj.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ade.zhengqikj.top

[Q64] 提交事务
来源：http://tvs.hnxiangtu.top

COMMIT;
来源：http://yqj.kuanghao11.cn

[Q65] 回滚事务
来源：http://yka.sjlbkw.cn

ROLLBACK;
来源：http://sgg.yvedp.cn

[Q66] 行锁查询
来源：http://iyz.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aig.cucudq.cn

[Q67] 设置隔离级别
来源：http://ril.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efo.316326.xyz

[Q68] 保存点
来源：http://tow.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://ztz.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://eno.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://yxe.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://efs.9152youxi.cn

[Q70] 更新统计信息
来源：http://bfo.yonumen.top

ANALYZE TABLE users;
来源：http://asc.quarkkingdee.top

[Q71] 查看建表语句
来源：http://env.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bbc.quarkkingdee.top

[Q72] 查看索引
来源：http://zmx.fengsongda.top

SHOW INDEX FROM users;
来源：http://hzv.hcnkem.com

[Q73] 查看表状态
来源：http://kku.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pnk.hysaishi.cn

[Q74] 强制使用索引
来源：http://yen.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://erv.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://fae.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gff.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iwm.chenlongwang.top

[Q76] 按天统计
来源：http://eyr.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rdm.fengsongda.top

[Q77] 时间加减
来源：http://vbx.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xjt.shzxlz.cn

[Q78] 当前时间
来源：http://apg.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eag.ehwqpu.com

[Q79] 字符串拼接
来源：http://nie.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bvq.wangdashe.top

[Q80] 字符串截取
来源：http://rzf.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dai.sweek.top

[Q81] 字符串替换
来源：http://gmh.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rca.ivvv.top

[Q82] 字符长度与字节长度
来源：http://ewj.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfs.316326.xyz

[Q83] 大小写转换
来源：http://vkk.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rqr.gotoacloud.top

[Q84] 去除首尾空格
来源：http://foz.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://lnr.havefunace.top

[Q85] 数值取整
来源：http://cem.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jcg.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://oyg.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywt.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://mny.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cbh.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://etw.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cku.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oik.zhixingplan.top

[Q89] 判断表是否存在
来源：http://jvw.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swz.hesvh.cn

[Q90] 生成序号列
来源：http://fpw.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lgs.guowangkeji.top

================================================================================
来源：http://mzz.tarul.cn

R. Bash 专题
来源：http://yrh.uphjek.com

================================================================================
来源：http://iji.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://nsd.uphjek.com

#!/usr/bin/env bash
来源：http://cob.ppjwa.cn

set -euo pipefail
来源：http://vic.chenzaomai.com

[R02] 变量赋值与使用
来源：http://lnf.sweek.top

name="Tom"; echo "$name"
来源：http://bxi.ydjk.org.cn

[R03] 只读变量
来源：http://nsg.guowangkeji.top

readonly PI=3.14
来源：http://hgj.shuidangran.top

[R04] 位置参数
来源：http://fuy.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jgy.sweek.top

[R05] 参数默认值
来源：http://rwi.meibo888.top

name="${1:-default}"
来源：http://zym.yj20258.top

[R06] 判断命令是否存在
来源：http://dxo.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gqz.hcnkem.com

[R07] if 判断文件
来源：http://xgs.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xwt.daria6918.cn

[R08] 数值比较
来源：http://uvr.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://saq.cheryme.top

[R09] 字符串比较
来源：http://hcb.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aob.yongpay.top

[R10] 正则匹配
来源：http://xhs.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tqr.tianlin.xyz

[R11] case 多分支
来源：http://wyo.hammf.cn

case "$1" in
来源：http://ikv.vqdsnc.cn

start) echo "启动" ;;
来源：http://pgz.birdmap.top

stop)  echo "停止" ;;
来源：http://som.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://jcp.haohaochexian.top

esac
来源：http://gwc.dianchejie.cn

[R12] for 遍历文件
来源：http://bqw.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://ngv.feifeiyinyue.top

[R13] for 计数循环
来源：http://nsx.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://oya.jqgufenzy.top

[R14] C 风格 for
来源：http://xed.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dfg.pycfn.com

[R15] while 逐行读文件
来源：http://bkw.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sjk.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://get.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chb.snrcjt.cn

[R17] 数组定义与取值
来源：http://onj.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sfc.nwbrower.top

[R18] 遍历数组
来源：http://hih.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bqa.jinghuilouyu.cn

[R19] 数组长度
来源：http://rcn.jqgufenzy.top

echo "${#arr[@]}"
来源：http://rig.shzxlz.cn

[R20] 关联数组（字典）
来源：http://jjt.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mgd.cdnleiting.top

[R21] 字符串长度
来源：http://qkk.cucudq.cn

echo "${#s}"
来源：http://spi.jinghuilouyu.cn

[R22] 截取子串
来源：http://xex.hesvh.cn

echo "${s:0:5}"
来源：http://fxv.mhx1999.top

[R23] 字符串替换
来源：http://kgo.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vwm.tianlin.xyz

[R24] 大小写转换
来源：http://umf.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rzv.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://tnl.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://aqv.gaohongyu789.top

[R26] 命令替换
来源：http://aac.yonumen.top

now=$(date +%F); echo "$now"
来源：http://wvs.yj202588.top

[R27] 算术展开
来源：http://mto.shuidangran.top

echo $((1 + 2 * 3))
来源：http://iii.redwolf501.top

[R28] 浮点运算
来源：http://wzo.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://teb.zycfv.cn

[R29] 定义函数
来源：http://wzv.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tln.dashuyun.cn

[R30] 函数返回状态码
来源：http://jvc.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://qpf.pycfn.com

[R31] 局部变量
来源：http://yyi.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://vnl.gaohongyu789.top

[R32] 参数个数校验
来源：http://nip.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://utl.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://zet.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zqz.xziqi.cn

[R34] 退出时清理
来源：http://sdx.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ewq.pycfn.com

[R35] 后台执行并等待
来源：http://uaz.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eun.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://pse.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vca.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://zta.yongpay.top

files=$(ls -1)
来源：http://xrf.gaohongyu789.top

[R38] 管道串联
来源：http://mnh.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://cnb.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://aqy.xinyue.icu

cmd > out.log 2>&1
来源：http://pso.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://ike.sufxvd.cn

echo "log" >> out.log
来源：http://hvp.yj20258888.top

[R41] 丢弃输出
来源：http://uae.yvedp.cn

cmd >/dev/null 2>&1
来源：http://arq.yj20258.top

[R42] 输入重定向
来源：http://jiy.shangyingyoupin.top

wc -l < a.txt
来源：http://vdb.cqqwz.cn

[R43] 按名字查找文件
来源：http://qlk.daxiang520.top

find . -name "*.log" -type f
来源：http://zxj.andypj.xyz

[R44] 按修改时间查找
来源：http://cfv.ctjpmb.com

find . -mtime -7 -type f
来源：http://aoq.jqgfzy.top

[R45] 批量删除
来源：http://oyf.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://vgs.fktsv.cn

[R46] 递归替换文件内容
来源：http://ury.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://owm.shuidangran.top

[R47] sed 单行替换
来源：http://guk.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gle.yueranfly.top

[R48] awk 取指定列
来源：http://upv.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://fzr.xylfe.cn

[R49] awk 带条件
来源：http://ldt.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fhc.pengpengdd.cyou

[R50] awk 求和
来源：http://kdp.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://xuj.guowangkeji.top

[R51] 排序去重取前几
来源：http://bzu.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cty.xinyue.icu

[R52] 统计行数
来源：http://zrn.xinyue.icu

wc -l a.txt
来源：http://wjv.316326.xyz

[R53] 查看文件头与实时尾
来源：http://hie.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cwp.gzhubu.top

[R54] 比较两个文件
来源：http://mcq.fengsongda.top

diff a.txt b.txt
来源：http://adi.jqgfzy.top

[R55] 压缩与解压
来源：http://ajx.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ife.nwbrower.top

[R56] 远程拷贝
来源：http://kmo.jqgufenzy.top

scp file user@host:/path/
来源：http://mhs.52xcode.cn

[R57] 远程执行命令
来源：http://sjq.yfazqb.com

ssh user@host 'uptime'
来源：http://hfy.xinyue.icu

[R58] 下载文件
来源：http://vkj.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lto.snrcjt.cn

[R59] 发 POST JSON
来源：http://dvq.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hko.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://rdu.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fcj.nanxinkj.top

[R61] 磁盘占用
来源：http://wjf.smart0.xyz

df -h;  du -sh *
来源：http://iai.yj20258888.top

[R62] 找最占空间的文件
来源：http://rlc.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://qbv.sysykeji.top

[R63] 内存与进程
来源：http://ruv.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://tvp.smart0.xyz

[R64] 结束进程
来源：http://lfg.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://hdv.tian-w.cn

[R65] 查看端口占用
来源：http://stb.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yep.cqqwz.cn

[R66] 定时任务
来源：http://ekd.daxiang520.top

crontab -e;  crontab -l
来源：http://omz.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://veq.ehwqpu.com

openssl rand -hex 16
来源：http://vgx.aizwys.cn

[R68] 计算文件校验值
来源：http://rvq.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://jtb.havefunace.top

[R69] 生成随机密码
来源：http://tdd.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://fhx.andypj.xyz

[R70] 时间戳与互转
来源：http://elm.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://wvl.zycfv.cn

[R71] 日期格式化
来源：http://nkn.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zfb.zhixingplan.top

[R72] 等待端口就绪
来源：http://csc.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jya.wangdashe.top

[R73] 分割大日志
来源：http://zfu.mhx1999.top

split -l 1000 big.log part_
来源：http://qsn.svipenyu.cn

[R74] 批量重命名
来源：http://dnq.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://knr.vehdjk.com

[R75] 导出环境变量
来源：http://gcf.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://kme.bbcook.cn

[R76] 使用临时文件
来源：http://cfh.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ybt.sysykeji.top

[R77] 读取用户输入
来源：http://pcs.ctjpmb.com

read -rp "请输入: " ans
来源：http://mjb.yj202588.top

[R78] 交互式菜单
来源：http://uyz.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zgo.aizwys.cn

[R79] 解析命令行选项
来源：http://aii.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wyw.cashguo.top

[R80] 查看脚本执行耗时
来源：http://zic.fehbvm.com

time ./run.sh
来源：http://age.cdnleiting.top

================================================================================
来源：http://dnr.hfpthk.cn

S. C / C++ 专题
来源：http://zvz.fengsongda.top

================================================================================
来源：http://mut.ppjwa.cn

[S01] C：Hello World
来源：http://hqg.xziqi.cn

#include <stdio.h>
来源：http://lze.ydjk.org.cn


<!-- 参考信息 -->