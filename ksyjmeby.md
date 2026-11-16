代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://cbq.cucudq.cn

[Q30] 分组统计
来源：http://fbe.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rvj.sxryk.cn

[Q31] 分组后过滤
来源：http://vbi.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xov.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://nej.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ajp.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jof.chenzaomai.com

[Q33] 多列分组
来源：http://ggr.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xug.daria6918.cn

[Q34] 每组取第一条
来源：http://pha.birdmap.top

SELECT * FROM (
来源：http://ahd.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zeh.chenlongwang.top

) t WHERE rn = 1;
来源：http://qvq.shangyingyoupin.top

[Q35] 内连接
来源：http://iik.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://amq.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://goj.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qqe.svipenyu.cn

[Q37] 右连接
来源：http://hcd.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfx.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://ozz.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ypu.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://taj.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jtc.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wnh.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xop.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fbh.jlsjyb.cn

[Q41] 多表连接
来源：http://hqd.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxz.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://dze.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://sfh.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://vth.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://eaf.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pxy.yvedp.cn

[Q43] 标量子查询
来源：http://ruk.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sej.fehbvm.com

[Q44] IN 子查询
来源：http://gly.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vsn.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://gtk.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ioh.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://wft.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://syj.hfpthk.cn

[Q47] 与平均值比较
来源：http://sec.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hmq.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://zis.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ggt.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://ikz.tian-w.cn

[Q49] 更新单行
来源：http://lnp.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://snv.xuetiantiany.cn

[Q50] 批量更新
来源：http://eyn.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ppq.yfazqb.com

[Q51] 用子查询更新
来源：http://knp.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dsb.guowangkeji.top

[Q52] 删除指定行
来源：http://sef.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://ybv.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://eku.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oga.pycfn.com

[Q54] 清空表
来源：http://bta.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://ajv.ivvv.top

[Q55] 排名（并列占位）
来源：http://zea.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfy.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://reb.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vyz.zhengqikj.top

[Q57] 行号
来源：http://jbi.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hfh.tian-w.cn

[Q58] 累计求和
来源：http://dqp.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kwg.jlsjyb.cn

[Q59] 分组内累计
来源：http://naw.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ils.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://ypk.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ygm.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://utu.52xcode.cn

[Q61] 移动平均
来源：http://ncc.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dos.hammf.cn

[Q62] 分组占比
来源：http://uoq.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wfq.kuanghao11.cn

[Q63] 开启事务
来源：http://lth.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eya.vqdsnc.cn

[Q64] 提交事务
来源：http://nmv.hammf.cn

COMMIT;
来源：http://qbp.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://dwm.xuanzx.com

ROLLBACK;
来源：http://uzp.ctjpmb.com

[Q66] 行锁查询
来源：http://dbx.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bda.chenzaomai.com

[Q67] 设置隔离级别
来源：http://kqb.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cht.yanxiufei.cn

[Q68] 保存点
来源：http://xcl.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://eol.sysykeji.top

ROLLBACK TO sp1;
来源：http://ohu.yangfankeji.com

[Q69] 查看执行计划
来源：http://edn.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fsx.haohaochexian.top

[Q70] 更新统计信息
来源：http://ifr.guowangkeji.top

ANALYZE TABLE users;
来源：http://vcp.xylfe.cn

[Q71] 查看建表语句
来源：http://zkk.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zdu.tian-w.cn

[Q72] 查看索引
来源：http://ypt.guannengcc.top

SHOW INDEX FROM users;
来源：http://nus.ydjk.org.cn

[Q73] 查看表状态
来源：http://qsi.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://fwq.316326.xyz

[Q74] 强制使用索引
来源：http://wil.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zym.yj20258888.top

[Q75] 日期格式化
来源：http://deb.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kin.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://thn.gotoacloud.top

[Q76] 按天统计
来源：http://wcr.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yju.316326.xyz

[Q77] 时间加减
来源：http://iee.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ynh.pengpengdd.cyou

[Q78] 当前时间
来源：http://zzv.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uma.xylfe.cn

[Q79] 字符串拼接
来源：http://jrg.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zfa.guannengcc.top

[Q80] 字符串截取
来源：http://gyq.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lga.cheryme.top

[Q81] 字符串替换
来源：http://txv.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rph.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://vov.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lyn.yfazqb.com

[Q83] 大小写转换
来源：http://wgn.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lxh.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://hme.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://mfy.jinqigufen.top

[Q85] 数值取整
来源：http://fmx.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qkk.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://pqk.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kdl.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://gif.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://llg.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://cot.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://skw.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vxs.snrcjt.cn

[Q89] 判断表是否存在
来源：http://tgm.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eav.daxiang520.top

[Q90] 生成序号列
来源：http://sug.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ezx.andypj.xyz

================================================================================
来源：http://fua.cashguo.top

R. Bash 专题
来源：http://eqm.shangyingyoupin.top

================================================================================
来源：http://msk.shuidangran.top

[R01] shebang 与严格模式
来源：http://dpo.yueranfly.top

#!/usr/bin/env bash
来源：http://jbk.chenzaomai.com

set -euo pipefail
来源：http://vlq.yuanzhike.top

[R02] 变量赋值与使用
来源：http://rfs.316326.xyz

name="Tom"; echo "$name"
来源：http://mmt.zycfv.cn

[R03] 只读变量
来源：http://hpl.uphjek.com

readonly PI=3.14
来源：http://xtz.ppjwa.cn

[R04] 位置参数
来源：http://kcn.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mwg.shanyushiyangtech.top

[R05] 参数默认值
来源：http://shn.havefunace.top

name="${1:-default}"
来源：http://uzh.cashguo.top

[R06] 判断命令是否存在
来源：http://lgt.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yyb.c1oappe.top

[R07] if 判断文件
来源：http://vdp.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://utc.316326.xyz

[R08] 数值比较
来源：http://zoe.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://dub.9152youxi.cn

[R09] 字符串比较
来源：http://joh.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gqi.fanxiaobao.xyz

[R10] 正则匹配
来源：http://mwb.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nge.haohaochexian.top

[R11] case 多分支
来源：http://put.xingfuxueyuan.xyz

case "$1" in
来源：http://brn.sysykeji.top

start) echo "启动" ;;
来源：http://lpu.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://keo.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://ocq.jinyuanbaomall.cn

esac
来源：http://odk.andypj.xyz

[R12] for 遍历文件
来源：http://mls.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://zrb.snrcjt.cn

[R13] for 计数循环
来源：http://dky.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://mzb.birdmap.top

[R14] C 风格 for
来源：http://vlo.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://avy.gaohongyu789.top

[R15] while 逐行读文件
来源：http://mcc.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qjc.shuidangran.top

[R16] until 等待条件
来源：http://swk.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cpg.hysaishi.cn

[R17] 数组定义与取值
来源：http://qab.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://pms.jlsjyb.cn

[R18] 遍历数组
来源：http://ofl.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsg.c1oappe.top

[R19] 数组长度
来源：http://fbc.bbcook.cn

echo "${#arr[@]}"
来源：http://ckl.havefunace.top

[R20] 关联数组（字典）
来源：http://taf.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvo.jinqigfzy.top

[R21] 字符串长度
来源：http://mgi.andypj.xyz

echo "${#s}"
来源：http://lra.tarul.cn

[R22] 截取子串
来源：http://iru.yj202588.top

echo "${s:0:5}"
来源：http://rno.yuanzhike.top

[R23] 字符串替换
来源：http://tvd.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qzr.mhx1999.top

[R24] 大小写转换
来源：http://wxg.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://brs.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://smb.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxs.pengpengdd.cyou

[R26] 命令替换
来源：http://iep.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://wuq.dashuyun.cn

[R27] 算术展开
来源：http://rof.mhx1999.top

echo $((1 + 2 * 3))
来源：http://bpz.316326.xyz

[R28] 浮点运算
来源：http://tll.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://kkm.bjfxy.top

[R29] 定义函数
来源：http://nod.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvv.quarkkingdee.top

[R30] 函数返回状态码
来源：http://izl.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://rhq.zycfv.cn

[R31] 局部变量
来源：http://fbh.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://lrz.quarkkingdee.top

[R32] 参数个数校验
来源：http://rzn.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bel.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://nhm.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vmn.tarul.cn

[R34] 退出时清理
来源：http://bke.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://vvo.tianlin.xyz

[R35] 后台执行并等待
来源：http://clq.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vnh.fzhhl.top

[R36] 并发执行多个任务
来源：http://zau.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vzt.tian-w.cn

[R37] 把输出赋给变量
来源：http://ifl.tarul.cn

files=$(ls -1)
来源：http://uvv.aibaodan.cn

[R38] 管道串联
来源：http://hgl.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://zgb.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://pri.316326.xyz

cmd > out.log 2>&1
来源：http://xcu.xziqi.cn

[R40] 追加写日志
来源：http://mho.pycfn.com

echo "log" >> out.log
来源：http://nvs.yangfankeji.com

[R41] 丢弃输出
来源：http://jig.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://rpf.jinqigfzy.top

[R42] 输入重定向
来源：http://bdx.jianghu66.top

wc -l < a.txt
来源：http://fpf.tianlin.xyz

[R43] 按名字查找文件
来源：http://vul.316326.xyz

find . -name "*.log" -type f
来源：http://ayo.haohaochexian.top

[R44] 按修改时间查找
来源：http://oxi.nanxuanxn.top

find . -mtime -7 -type f
来源：http://lhr.xuanzx.com

[R45] 批量删除
来源：http://cse.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://toa.jyoumei.cn

[R46] 递归替换文件内容
来源：http://ljw.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cgh.vehdjk.com

[R47] sed 单行替换
来源：http://wlg.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tlf.hongshengwenyu.top

[R48] awk 取指定列
来源：http://wca.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://lvw.fktsv.cn

[R49] awk 带条件
来源：http://bep.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://suu.guowangkeji.top

[R50] awk 求和
来源：http://wka.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://tct.ybcxt.top

[R51] 排序去重取前几
来源：http://nxy.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qez.mhx1999.top

[R52] 统计行数
来源：http://hfn.zdqjudy.top

wc -l a.txt
来源：http://smt.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://ubn.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://emq.fktsv.cn

[R54] 比较两个文件
来源：http://upb.0kj1m.cn

diff a.txt b.txt
来源：http://vat.cheryme.top

[R55] 压缩与解压
来源：http://ppi.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nxp.gotoacloud.top

[R56] 远程拷贝
来源：http://jal.bjfxy.top

scp file user@host:/path/
来源：http://iac.gogol.net.cn

[R57] 远程执行命令
来源：http://ihu.hysaishi.cn

ssh user@host 'uptime'
来源：http://ube.hcnkem.com

[R58] 下载文件
来源：http://ugl.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gcv.dianchejie.cn

[R59] 发 POST JSON
来源：http://myv.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fpc.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://sbw.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sux.yj20258888.top

[R61] 磁盘占用
来源：http://vyl.ctjpmb.com

df -h;  du -sh *
来源：http://beg.xylfe.cn

[R62] 找最占空间的文件
来源：http://ewx.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://fhf.gaohongyu789.top

[R63] 内存与进程
来源：http://ynb.pycfn.com

free -h;  ps aux | grep nginx
来源：http://cpm.jinghuilouyu.cn

[R64] 结束进程
来源：http://qfh.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://fjd.shzxlz.cn

[R65] 查看端口占用
来源：http://awd.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yut.jyoumei.cn

[R66] 定时任务
来源：http://syq.fzhhl.top

crontab -e;  crontab -l
来源：http://jks.meibo888.top

[R67] 生成随机十六进制串
来源：http://mtw.zhixingplan.top

openssl rand -hex 16
来源：http://qxz.svipenyu.cn

[R68] 计算文件校验值
来源：http://yah.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ngz.bbcook.cn

[R69] 生成随机密码
来源：http://vov.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://yxy.hysaishi.cn

[R70] 时间戳与互转
来源：http://lis.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://dhv.dianchejie.cn

[R71] 日期格式化
来源：http://ijt.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zmh.jianghu66.top

[R72] 等待端口就绪
来源：http://cxp.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sji.cashguo.top

[R73] 分割大日志
来源：http://zzi.snrcjt.cn

split -l 1000 big.log part_
来源：http://ihc.zhoulong.xyz

[R74] 批量重命名
来源：http://qtf.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysc.zhongyouzk.top

[R75] 导出环境变量
来源：http://phs.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://gmb.vehdjk.com

[R76] 使用临时文件
来源：http://kdz.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xgb.shuidangran.top

[R77] 读取用户输入
来源：http://epj.gogol.net.cn

read -rp "请输入: " ans
来源：http://gzu.xuanzx.com

[R78] 交互式菜单
来源：http://fqs.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://krn.hywenlv.cn

[R79] 解析命令行选项
来源：http://cko.xuetiantiany.cn


<!-- 参考信息 -->