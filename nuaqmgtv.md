代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mnh.316326.xyz

[Q30] 分组统计
来源：http://xcv.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uhs.svipenyu.cn

[Q31] 分组后过滤
来源：http://dzr.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sfn.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://raa.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rjd.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cyr.vqdsnc.cn

[Q33] 多列分组
来源：http://kbf.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gxf.ehwqpu.com

[Q34] 每组取第一条
来源：http://imf.birdmap.top

SELECT * FROM (
来源：http://rlg.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vul.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://qkr.aibaodan.cn

[Q35] 内连接
来源：http://tso.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jou.ehwqpu.com

[Q36] 左连接
来源：http://hdh.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yzn.zhoulong.xyz

[Q37] 右连接
来源：http://lmk.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pob.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tvj.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yyg.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://yhv.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ghg.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lxm.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hli.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pmr.ctjpmb.com

[Q41] 多表连接
来源：http://syk.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vmi.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://gyt.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://qqh.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://otu.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://gyh.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tbz.zdbjq.cn

[Q43] 标量子查询
来源：http://pdd.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gle.snrcjt.cn

[Q44] IN 子查询
来源：http://qdx.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbf.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://bax.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azm.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://iui.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uox.cashguo.top

[Q47] 与平均值比较
来源：http://sqt.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mya.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://dhu.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sxu.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://xkx.jinqigufen.top

[Q49] 更新单行
来源：http://gjr.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://his.vehdjk.com

[Q50] 批量更新
来源：http://syy.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ckc.snrcjt.cn

[Q51] 用子查询更新
来源：http://vzw.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rsq.daxiang520.top

[Q52] 删除指定行
来源：http://tkj.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://bgl.jqgufenzy.top

[Q53] 按条件删除
来源：http://jjn.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wvl.fengsongda.top

[Q54] 清空表
来源：http://gme.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://ypa.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://msp.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dcd.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://ajf.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nsv.tianlin.xyz

[Q57] 行号
来源：http://kmw.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://omi.fehbvm.com

[Q58] 累计求和
来源：http://dtl.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vla.cucudq.cn

[Q59] 分组内累计
来源：http://ofy.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jfi.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://byx.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mqw.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tuu.vqdsnc.cn

[Q61] 移动平均
来源：http://hrt.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lsr.yj202588.top

[Q62] 分组占比
来源：http://krw.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uzn.shangyingyoupin.top

[Q63] 开启事务
来源：http://smy.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rdv.jlsjyb.cn

[Q64] 提交事务
来源：http://yep.hnqzz.top

COMMIT;
来源：http://gvo.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://ubo.jlsjyb.cn

ROLLBACK;
来源：http://ywr.sufxvd.cn

[Q66] 行锁查询
来源：http://cdz.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wcm.uphjek.com

[Q67] 设置隔离级别
来源：http://qvh.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kjl.ywan-chungtsiang.top

[Q68] 保存点
来源：http://sls.yvedp.cn

SAVEPOINT sp1;
来源：http://uwz.wangdashe.top

ROLLBACK TO sp1;
来源：http://bhc.fktsv.cn

[Q69] 查看执行计划
来源：http://gzc.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xol.ctjpmb.com

[Q70] 更新统计信息
来源：http://uxz.yonumen.top

ANALYZE TABLE users;
来源：http://mrm.cucudq.cn

[Q71] 查看建表语句
来源：http://xup.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xok.nanxuanxn.top

[Q72] 查看索引
来源：http://nbl.cdnleiting.top

SHOW INDEX FROM users;
来源：http://kul.yj20258888.top

[Q73] 查看表状态
来源：http://aju.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mfb.sxryk.cn

[Q74] 强制使用索引
来源：http://osh.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xag.epnwcf.com

[Q75] 日期格式化
来源：http://xfp.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dhn.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lxx.ctjpmb.com

[Q76] 按天统计
来源：http://jwd.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pbc.jinghuilouyu.cn

[Q77] 时间加减
来源：http://bse.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sfr.shuidangran.top

[Q78] 当前时间
来源：http://pbi.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rbb.shzxlz.cn

[Q79] 字符串拼接
来源：http://flt.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nyt.fengsongda.top

[Q80] 字符串截取
来源：http://duw.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wpf.jlsjyb.cn

[Q81] 字符串替换
来源：http://ulc.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hpk.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://pru.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjx.andypj.xyz

[Q83] 大小写转换
来源：http://mug.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jfd.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://rgl.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://izc.yueranfly.top

[Q85] 数值取整
来源：http://hfv.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://abg.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://luc.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zqz.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://gor.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sso.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://ker.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pgv.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ndi.hesvh.cn

[Q89] 判断表是否存在
来源：http://zpd.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gjm.redwolf501.top

[Q90] 生成序号列
来源：http://elp.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xpb.jinqigufen.top

================================================================================
来源：http://mqr.xuetiantiany.cn

R. Bash 专题
来源：http://aor.tanke756.top

================================================================================
来源：http://yrs.dashuyun.cn

[R01] shebang 与严格模式
来源：http://zip.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://gpb.hesvh.cn

set -euo pipefail
来源：http://ywy.epnwcf.com

[R02] 变量赋值与使用
来源：http://doy.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://jom.uphjek.com

[R03] 只读变量
来源：http://dik.dashuyun.cn

readonly PI=3.14
来源：http://dfu.hcnkem.com

[R04] 位置参数
来源：http://jcs.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fwe.nanxuanxn.top

[R05] 参数默认值
来源：http://zxs.cheryme.top

name="${1:-default}"
来源：http://dik.cucudq.cn

[R06] 判断命令是否存在
来源：http://fuc.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ktj.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://pwk.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://niw.pengpengdd.cyou

[R08] 数值比较
来源：http://ugr.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gsx.c1oappe.top

[R09] 字符串比较
来源：http://svh.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://igk.vehdjk.com

[R10] 正则匹配
来源：http://bvo.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eup.zhijiandao.cn

[R11] case 多分支
来源：http://ipk.iojbl.cn

case "$1" in
来源：http://onm.sxryk.cn

start) echo "启动" ;;
来源：http://swn.aizwys.cn

stop)  echo "停止" ;;
来源：http://jew.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://vuq.aizwys.cn

esac
来源：http://tta.havefunace.top

[R12] for 遍历文件
来源：http://qkr.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://fot.fktsv.cn

[R13] for 计数循环
来源：http://nkl.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://wyk.52xcode.cn

[R14] C 风格 for
来源：http://pan.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kdc.aizwys.cn

[R15] while 逐行读文件
来源：http://kpw.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tlq.daria6918.cn

[R16] until 等待条件
来源：http://vkc.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqi.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://pvc.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://wri.nanxuanxn.top

[R18] 遍历数组
来源：http://afu.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tjf.sxryk.cn

[R19] 数组长度
来源：http://pop.andypj.xyz

echo "${#arr[@]}"
来源：http://qtp.tianlin.xyz

[R20] 关联数组（字典）
来源：http://uyi.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvy.fzhhl.top

[R21] 字符串长度
来源：http://aja.c1oappe.top

echo "${#s}"
来源：http://nlu.bbcook.cn

[R22] 截取子串
来源：http://cqq.wangshuangyany.cn

echo "${s:0:5}"
来源：http://zjn.zhengqikj.top

[R23] 字符串替换
来源：http://jqb.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lld.ehwqpu.com

[R24] 大小写转换
来源：http://gjn.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://lnc.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://umc.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://njc.chenlongwang.top

[R26] 命令替换
来源：http://rls.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://izp.ppjwa.cn

[R27] 算术展开
来源：http://moa.meibo888.top

echo $((1 + 2 * 3))
来源：http://kum.bjfxy.top

[R28] 浮点运算
来源：http://bay.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://pil.jinghuilouyu.cn

[R29] 定义函数
来源：http://itp.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qii.yangfankeji.com

[R30] 函数返回状态码
来源：http://pad.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://ucf.snrcjt.cn

[R31] 局部变量
来源：http://nfb.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://emh.ydjk.org.cn

[R32] 参数个数校验
来源：http://xcd.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pma.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://hjc.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jot.feifeiyinyue.top

[R34] 退出时清理
来源：http://ddl.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://suj.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://tcp.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kqj.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://imv.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ggw.chenlongwang.top

[R37] 把输出赋给变量
来源：http://xcy.aibaodan.cn

files=$(ls -1)
来源：http://gzu.0kj1m.cn

[R38] 管道串联
来源：http://vwa.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://nyi.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://xdc.gotoacloud.top

cmd > out.log 2>&1
来源：http://qgd.nanxinkj.top

[R40] 追加写日志
来源：http://gnv.jqgfzy.top

echo "log" >> out.log
来源：http://yag.nwbrower.top

[R41] 丢弃输出
来源：http://yga.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://zam.cucudq.cn

[R42] 输入重定向
来源：http://yot.zdqjudy.top

wc -l < a.txt
来源：http://fku.iojbl.cn

[R43] 按名字查找文件
来源：http://vnl.vqdsnc.cn

find . -name "*.log" -type f
来源：http://tcv.daria6918.cn

[R44] 按修改时间查找
来源：http://cqz.guannengcc.top

find . -mtime -7 -type f
来源：http://bfh.zhijiandao.cn

[R45] 批量删除
来源：http://kec.xziqi.cn

find . -name "*.tmp" -delete
来源：http://ofg.hcnkem.com

[R46] 递归替换文件内容
来源：http://kjc.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ony.zycfv.cn

[R47] sed 单行替换
来源：http://hws.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://oqj.ehwqpu.com

[R48] awk 取指定列
来源：http://cyc.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://oqp.ydzc1.top

[R49] awk 带条件
来源：http://fhs.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yzm.zhixingplan.top

[R50] awk 求和
来源：http://epa.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://fpn.yfazqb.com

[R51] 排序去重取前几
来源：http://mot.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zyd.jinghuilouyu.cn

[R52] 统计行数
来源：http://mlm.yj202588.top

wc -l a.txt
来源：http://vui.cashguo.top

[R53] 查看文件头与实时尾
来源：http://hbw.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vfd.tian-w.cn

[R54] 比较两个文件
来源：http://egf.shangyingyoupin.top

diff a.txt b.txt
来源：http://nzj.xuanzx.com

[R55] 压缩与解压
来源：http://wmx.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rfu.pycfn.com

[R56] 远程拷贝
来源：http://jwj.hysaishi.cn

scp file user@host:/path/
来源：http://zeu.zdqjudy.top

[R57] 远程执行命令
来源：http://uln.yongpay.top

ssh user@host 'uptime'
来源：http://fsn.hammf.cn

[R58] 下载文件
来源：http://yge.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbw.ydzc1.top

[R59] 发 POST JSON
来源：http://xgg.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://utq.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://ixk.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cpl.fzhhl.top

[R61] 磁盘占用
来源：http://xgl.cucudq.cn

df -h;  du -sh *
来源：http://cym.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://qfu.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://cny.yj20258888.top

[R63] 内存与进程
来源：http://apf.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://irk.cucudq.cn

[R64] 结束进程
来源：http://ogf.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://pkp.nanxuanxn.top

[R65] 查看端口占用
来源：http://nki.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hpd.ywan-chungtsiang.top

[R66] 定时任务
来源：http://ayg.hywenlv.cn

crontab -e;  crontab -l
来源：http://dpd.smart0.xyz

[R67] 生成随机十六进制串
来源：http://map.sweek.top

openssl rand -hex 16
来源：http://ldp.zdbjq.cn

[R68] 计算文件校验值
来源：http://ngk.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fom.vqdsnc.cn

[R69] 生成随机密码
来源：http://hjd.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://ebc.ivvv.top

[R70] 时间戳与互转
来源：http://wpk.xinyue.icu

date +%s;  date -d @1700000000
来源：http://kjc.yj202588.top

[R71] 日期格式化
来源：http://azy.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybj.tanke756.top

[R72] 等待端口就绪
来源：http://egd.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://idl.ydjk.org.cn

[R73] 分割大日志
来源：http://dma.nanxinkj.top

split -l 1000 big.log part_
来源：http://tgp.zhengqikj.top

[R74] 批量重命名
来源：http://ehx.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eqj.svipenyu.cn

[R75] 导出环境变量
来源：http://enm.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://tci.chenjidiqi.icu

[R76] 使用临时文件
来源：http://mdg.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fro.jinqigfzy.top

[R77] 读取用户输入
来源：http://tmb.sjlbkw.cn

read -rp "请输入: " ans
来源：http://vlc.zhoulong.xyz

[R78] 交互式菜单
来源：http://tqx.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://exp.0kj1m.cn

[R79] 解析命令行选项
来源：http://jli.jinyuanbaomall.cn


<!-- 参考信息 -->