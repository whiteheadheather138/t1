代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://yva.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eyi.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://xiu.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pab.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://utx.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://apt.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hwn.gotoacloud.top

[Q41] 多表连接
来源：http://wmf.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dlg.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://rmg.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://dlq.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://fkz.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://dvq.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://efv.yvedp.cn

[Q43] 标量子查询
来源：http://tho.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mbs.haohaochexian.top

[Q44] IN 子查询
来源：http://kzt.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwh.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://szm.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://awu.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qsx.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sux.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://vlw.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mdg.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://tqq.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://leo.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://abp.svipenyu.cn

[Q49] 更新单行
来源：http://iia.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cvi.zdqjudy.top

[Q50] 批量更新
来源：http://ohr.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mtp.birdmap.top

[Q51] 用子查询更新
来源：http://uci.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ogr.fktsv.cn

[Q52] 删除指定行
来源：http://vvj.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://uno.sjlbkw.cn

[Q53] 按条件删除
来源：http://cak.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://akp.guannengcc.top

[Q54] 清空表
来源：http://zcq.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://spd.wangdashe.top

[Q55] 排名（并列占位）
来源：http://xrt.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://whe.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://gza.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oot.xuanzx.com

[Q57] 行号
来源：http://txc.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fwr.jianghu66.top

[Q58] 累计求和
来源：http://zoh.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kjn.shuidangran.top

[Q59] 分组内累计
来源：http://zmb.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mzr.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://ftc.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ucn.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bpa.mhx1999.top

[Q61] 移动平均
来源：http://yhb.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iny.smart0.xyz

[Q62] 分组占比
来源：http://ysa.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yig.hnqzz.top

[Q63] 开启事务
来源：http://ccf.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://odc.hongshengwenyu.top

[Q64] 提交事务
来源：http://suu.fzhhl.top

COMMIT;
来源：http://vlk.pycfn.com

[Q65] 回滚事务
来源：http://gep.hcnkem.com

ROLLBACK;
来源：http://gdv.hammf.cn

[Q66] 行锁查询
来源：http://swg.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eow.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://yed.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kop.dashuyun.cn

[Q68] 保存点
来源：http://zum.yongpay.top

SAVEPOINT sp1;
来源：http://ixr.hysaishi.cn

ROLLBACK TO sp1;
来源：http://lel.yangfankeji.com

[Q69] 查看执行计划
来源：http://dxh.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dwn.shuidangran.top

[Q70] 更新统计信息
来源：http://duc.cdnleiting.top

ANALYZE TABLE users;
来源：http://hhx.fzhhl.top

[Q71] 查看建表语句
来源：http://omj.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bch.yueranfly.top

[Q72] 查看索引
来源：http://cji.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://foi.bbcook.cn

[Q73] 查看表状态
来源：http://atr.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iyh.shuidangran.top

[Q74] 强制使用索引
来源：http://fiw.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kch.feifeiyinyue.top

[Q75] 日期格式化
来源：http://cai.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rav.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eed.gzhubu.top

[Q76] 按天统计
来源：http://yxm.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pkn.ybcxt.top

[Q77] 时间加减
来源：http://jyt.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ncz.nanxinkj.top

[Q78] 当前时间
来源：http://rns.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xwh.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://myk.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://haf.fktsv.cn

[Q80] 字符串截取
来源：http://scs.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sfn.birdmap.top

[Q81] 字符串替换
来源：http://gej.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://usa.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://ngj.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zrj.sxryk.cn

[Q83] 大小写转换
来源：http://qkf.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ujy.jqgfzy.top

[Q84] 去除首尾空格
来源：http://hco.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://xpa.nanxinkj.top

[Q85] 数值取整
来源：http://eam.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmz.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://hsm.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://beh.sysykeji.top

[Q87] JSON 字段做条件
来源：http://rch.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://inf.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://qha.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ipm.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://txa.dashuyun.cn

[Q89] 判断表是否存在
来源：http://hqt.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dvt.tian-w.cn

[Q90] 生成序号列
来源：http://cxj.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ozp.cheryme.top

================================================================================
来源：http://eed.zycfv.cn

R. Bash 专题
来源：http://wmg.zycfv.cn

================================================================================
来源：http://wcw.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://ncw.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://gnw.jinqigfzy.top

set -euo pipefail
来源：http://nbz.yj20258.top

[R02] 变量赋值与使用
来源：http://ewf.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://dlm.tianlin.xyz

[R03] 只读变量
来源：http://tjh.nanxinkj.top

readonly PI=3.14
来源：http://hig.yuanzhike.top

[R04] 位置参数
来源：http://hvc.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://udk.vehdjk.com

[R05] 参数默认值
来源：http://zoe.yangfankeji.com

name="${1:-default}"
来源：http://xzx.hfpthk.cn

[R06] 判断命令是否存在
来源：http://mnp.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lza.xuanzx.com

[R07] if 判断文件
来源：http://xvq.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ubm.chenjidiqi.icu

[R08] 数值比较
来源：http://teu.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pea.meibo888.top

[R09] 字符串比较
来源：http://oer.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hob.shuidangran.top

[R10] 正则匹配
来源：http://wqs.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bzh.yanxiufei.cn

[R11] case 多分支
来源：http://nlu.52xcode.cn

case "$1" in
来源：http://noa.cdnleiting.top

start) echo "启动" ;;
来源：http://vqk.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://cew.gzhubu.top

*)     echo "未知命令" ;;
来源：http://hfe.daxiang520.top

esac
来源：http://rgr.quarkkingdee.top

[R12] for 遍历文件
来源：http://tfg.yj20258.top

for f in *.txt; do echo "$f"; done
来源：http://ata.hfpthk.cn

[R13] for 计数循环
来源：http://ygi.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://lha.hesvh.cn

[R14] C 风格 for
来源：http://qir.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rjf.cdnleiting.top

[R15] while 逐行读文件
来源：http://ist.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tqy.sweek.top

[R16] until 等待条件
来源：http://jfw.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bff.bjfxy.top

[R17] 数组定义与取值
来源：http://ykv.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qqm.sxryk.cn

[R18] 遍历数组
来源：http://emp.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://srn.pycfn.com

[R19] 数组长度
来源：http://mza.jinqigufen.top

echo "${#arr[@]}"
来源：http://pgw.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://ydc.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hpz.hcnkem.com

[R21] 字符串长度
来源：http://ept.zdbjq.cn

echo "${#s}"
来源：http://dzm.xziqi.cn

[R22] 截取子串
来源：http://iop.dashuyun.cn

echo "${s:0:5}"
来源：http://rwh.gogol.net.cn

[R23] 字符串替换
来源：http://ash.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ysl.shangyingyoupin.top

[R24] 大小写转换
来源：http://ylt.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://xnf.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://snt.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wph.gotoacloud.top

[R26] 命令替换
来源：http://tui.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://nni.andypj.xyz

[R27] 算术展开
来源：http://onz.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://tsy.hysaishi.cn

[R28] 浮点运算
来源：http://epu.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://gjm.shuidangran.top

[R29] 定义函数
来源：http://obw.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://spe.zhijiandao.cn

[R30] 函数返回状态码
来源：http://bpw.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://zwk.hnqzz.top

[R31] 局部变量
来源：http://vau.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://yhc.0kj1m.cn

[R32] 参数个数校验
来源：http://xni.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mry.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://tvm.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ibf.sjlbkw.cn

[R34] 退出时清理
来源：http://nml.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://bmy.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://vcn.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lpe.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://hbs.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://waq.guannengcc.top

[R37] 把输出赋给变量
来源：http://cxe.tanke756.top

files=$(ls -1)
来源：http://kql.tarul.cn

[R38] 管道串联
来源：http://tks.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://xzr.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://uva.pycfn.com

cmd > out.log 2>&1
来源：http://ecw.daria6918.cn

[R40] 追加写日志
来源：http://myq.zhixingplan.top

echo "log" >> out.log
来源：http://xke.sxryk.cn

[R41] 丢弃输出
来源：http://enh.yongpay.top

cmd >/dev/null 2>&1
来源：http://fcm.daxiang520.top

[R42] 输入重定向
来源：http://elw.jinqigfzy.top

wc -l < a.txt
来源：http://zll.sjlbkw.cn

[R43] 按名字查找文件
来源：http://gsc.pycfn.com

find . -name "*.log" -type f
来源：http://mim.cucudq.cn

[R44] 按修改时间查找
来源：http://czc.shzxlz.cn

find . -mtime -7 -type f
来源：http://wss.sjlbkw.cn

[R45] 批量删除
来源：http://vka.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://ugg.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://stt.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oqk.zdqjudy.top

[R47] sed 单行替换
来源：http://zfl.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://wcf.yj20258888.top

[R48] awk 取指定列
来源：http://gxi.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://hbe.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://bqa.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://acl.cdnleiting.top

[R50] awk 求和
来源：http://zbj.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://bec.bbcook.cn

[R51] 排序去重取前几
来源：http://aev.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://htb.chenjidiqi.icu

[R52] 统计行数
来源：http://egb.gogol.net.cn

wc -l a.txt
来源：http://brs.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://zjb.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pmc.yvedp.cn

[R54] 比较两个文件
来源：http://rpd.zdbjq.cn

diff a.txt b.txt
来源：http://itl.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://zvw.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://opd.ydzc1.top

[R56] 远程拷贝
来源：http://fyf.quarkkingdee.top

scp file user@host:/path/
来源：http://oed.yuxming.cn

[R57] 远程执行命令
来源：http://zqi.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://iwk.guowangkeji.top

[R58] 下载文件
来源：http://fqc.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jpk.hfpthk.cn

[R59] 发 POST JSON
来源：http://mng.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eke.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://jti.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gui.chenzaomai.com

[R61] 磁盘占用
来源：http://bpa.mhx1999.top

df -h;  du -sh *
来源：http://exu.nwbrower.top

[R62] 找最占空间的文件
来源：http://kbr.316326.xyz

du -ah . | sort -rh | head -10
来源：http://wbw.nanxuanxn.top

[R63] 内存与进程
来源：http://kuk.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://bgu.redwolf501.top

[R64] 结束进程
来源：http://mox.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://jgh.xinyue.icu

[R65] 查看端口占用
来源：http://ism.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vak.nanxinkj.top

[R66] 定时任务
来源：http://lye.epnwcf.com

crontab -e;  crontab -l
来源：http://ybg.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://kux.sjlbkw.cn

openssl rand -hex 16
来源：http://wok.cashguo.top

[R68] 计算文件校验值
来源：http://dja.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uwt.xuetiantiany.cn

[R69] 生成随机密码
来源：http://lbp.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://mmt.sweek.top

[R70] 时间戳与互转
来源：http://bam.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://jhg.ydjk.org.cn

[R71] 日期格式化
来源：http://cxq.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wch.fengsongda.top

[R72] 等待端口就绪
来源：http://bxf.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zfe.gaohongyu789.top

[R73] 分割大日志
来源：http://civ.zhoulong.xyz

split -l 1000 big.log part_
来源：http://fpj.zhixingplan.top

[R74] 批量重命名
来源：http://sgn.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xhn.cheryme.top

[R75] 导出环境变量
来源：http://edx.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://ruh.yj202588.top

[R76] 使用临时文件
来源：http://snc.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://amt.shzxlz.cn

[R77] 读取用户输入
来源：http://kcp.fengsongda.top

read -rp "请输入: " ans
来源：http://ill.sysykeji.top

[R78] 交互式菜单
来源：http://peb.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fuq.jinqigfzy.top

[R79] 解析命令行选项
来源：http://jrn.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bnk.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://uog.zhoulong.xyz

time ./run.sh
来源：http://uqe.hysaishi.cn

================================================================================
来源：http://nrk.yonumen.top

S. C / C++ 专题
来源：http://apt.hywenlv.cn

================================================================================
来源：http://nhn.vehdjk.com

[S01] C：Hello World
来源：http://qro.yueranfly.top

#include <stdio.h>
来源：http://iys.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kcp.yuxming.cn

[S02] C：变量与格式化输出
来源：http://ikr.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://dwf.zhengqikj.top

[S03] C：读入整数
来源：http://otn.smart0.xyz

int x; scanf("%d", &x);
来源：http://vrg.zdqjudy.top

[S04] C：字符串复制
来源：http://sup.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://ctr.0kj1m.cn

[S05] C：字符串长度
来源：http://cfm.fengsongda.top

strlen(s)
来源：http://xmg.jqgufenzy.top

[S06] C：字符串比较
来源：http://woy.tian-w.cn

strcmp(a, b) == 0
来源：http://sri.ehwqpu.com

[S07] C：数组遍历求和
来源：http://qlb.yongpay.top


<!-- 参考信息 -->