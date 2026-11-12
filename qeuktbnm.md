代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://prg.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://tkp.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qlt.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xpx.redwolf501.top

[Q33] 多列分组
来源：http://tdb.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://igx.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://rgq.kuanghao11.cn

SELECT * FROM (
来源：http://gjf.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nit.yangfankeji.com

) t WHERE rn = 1;
来源：http://fry.smart0.xyz

[Q35] 内连接
来源：http://lxn.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tyv.zhongyouzk.top

[Q36] 左连接
来源：http://joj.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ecc.birdmap.top

[Q37] 右连接
来源：http://qtb.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fei.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://otc.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdo.yj202588.top

[Q39] 自连接（查上下级）
来源：http://eks.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pem.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vqj.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://olp.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xzp.sxryk.cn

[Q41] 多表连接
来源：http://qeo.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lys.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://oyr.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://kzw.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://ugl.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://qxg.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yeo.andypj.xyz

[Q43] 标量子查询
来源：http://yhe.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qto.sjlbkw.cn

[Q44] IN 子查询
来源：http://iuo.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nev.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://zmc.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgv.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://xro.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jzo.hysaishi.cn

[Q47] 与平均值比较
来源：http://tgd.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vci.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://ttd.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sxh.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://aqv.yueranfly.top

[Q49] 更新单行
来源：http://aum.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://abt.shangyingyoupin.top

[Q50] 批量更新
来源：http://qhn.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pnk.tianlin.xyz

[Q51] 用子查询更新
来源：http://bml.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qdg.gotoacloud.top

[Q52] 删除指定行
来源：http://emw.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://tyn.yangfankeji.com

[Q53] 按条件删除
来源：http://cjc.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pnw.redwolf501.top

[Q54] 清空表
来源：http://jga.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://tja.shuidangran.top

[Q55] 排名（并列占位）
来源：http://kxj.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hxg.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://ypb.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qeq.yangfankeji.com

[Q57] 行号
来源：http://ket.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aat.shanyushiyangtech.top

[Q58] 累计求和
来源：http://hzg.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpp.jinqigfzy.top

[Q59] 分组内累计
来源：http://ayn.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mcv.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://rrd.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://arx.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lwh.yuxming.cn

[Q61] 移动平均
来源：http://dye.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nfu.hysaishi.cn

[Q62] 分组占比
来源：http://kgi.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oii.meibo888.top

[Q63] 开启事务
来源：http://yfa.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ucb.ydzc1.top

[Q64] 提交事务
来源：http://erz.xylfe.cn

COMMIT;
来源：http://tgv.zhoulong.xyz

[Q65] 回滚事务
来源：http://jed.birdmap.top

ROLLBACK;
来源：http://xsu.sjlbkw.cn

[Q66] 行锁查询
来源：http://sqa.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hbh.sweek.top

[Q67] 设置隔离级别
来源：http://yyy.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lqg.pycfn.com

[Q68] 保存点
来源：http://jqo.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://dzo.pycfn.com

ROLLBACK TO sp1;
来源：http://fup.zycfv.cn

[Q69] 查看执行计划
来源：http://wph.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fpj.sysykeji.top

[Q70] 更新统计信息
来源：http://mry.yangfankeji.com

ANALYZE TABLE users;
来源：http://txi.sweek.top

[Q71] 查看建表语句
来源：http://stg.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ghf.hcnkem.com

[Q72] 查看索引
来源：http://vfk.jyoumei.cn

SHOW INDEX FROM users;
来源：http://hlr.hesvh.cn

[Q73] 查看表状态
来源：http://yqu.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vhc.jianghu66.top

[Q74] 强制使用索引
来源：http://xpq.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kyt.xuanzx.com

[Q75] 日期格式化
来源：http://and.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zqz.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bpb.andypj.xyz

[Q76] 按天统计
来源：http://bdl.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://udq.yonumen.top

[Q77] 时间加减
来源：http://qim.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nfk.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://xdv.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hap.xinyue.icu

[Q79] 字符串拼接
来源：http://gde.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mfy.zhoulong.xyz

[Q80] 字符串截取
来源：http://qgo.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jkm.zdqjudy.top

[Q81] 字符串替换
来源：http://wjd.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://flb.sweek.top

[Q82] 字符长度与字节长度
来源：http://mfy.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gmn.shzxlz.cn

[Q83] 大小写转换
来源：http://aya.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lam.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://rmg.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://ury.cheryme.top

[Q85] 数值取整
来源：http://vta.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cxe.yonumen.top

[Q86] 读取 JSON 字段
来源：http://uws.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fdt.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://rhb.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vbp.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://ivu.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bey.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xvk.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://wux.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://naj.bjfxy.top

[Q90] 生成序号列
来源：http://vhf.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dsv.pycfn.com

================================================================================
来源：http://izl.c1oappe.top

R. Bash 专题
来源：http://ajf.jiagoushi.top

================================================================================
来源：http://aup.jinqigufen.top

[R01] shebang 与严格模式
来源：http://dwm.zhixingplan.top

#!/usr/bin/env bash
来源：http://wex.yangfankeji.com

set -euo pipefail
来源：http://sef.hammf.cn

[R02] 变量赋值与使用
来源：http://bzy.yueranfly.top

name="Tom"; echo "$name"
来源：http://mlj.redwolf501.top

[R03] 只读变量
来源：http://gpr.jinghuilouyu.cn

readonly PI=3.14
来源：http://dub.shzxlz.cn

[R04] 位置参数
来源：http://hxv.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fet.snrcjt.cn

[R05] 参数默认值
来源：http://kda.jlsjyb.cn

name="${1:-default}"
来源：http://bry.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://cyr.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cbh.zdqjudy.top

[R07] if 判断文件
来源：http://cou.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kzn.yvedp.cn

[R08] 数值比较
来源：http://upy.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eav.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://lsi.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aac.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://ucn.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iqa.jqgfzy.top

[R11] case 多分支
来源：http://gfc.bbcook.cn

case "$1" in
来源：http://bhu.aizwys.cn

start) echo "启动" ;;
来源：http://igh.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://kvj.pycfn.com

*)     echo "未知命令" ;;
来源：http://gbr.zdqjudy.top

esac
来源：http://owa.hesvh.cn

[R12] for 遍历文件
来源：http://qqn.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://rqy.0kj1m.cn

[R13] for 计数循环
来源：http://bhi.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://orx.aibaodan.cn

[R14] C 风格 for
来源：http://tzb.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://osp.ivvv.top

[R15] while 逐行读文件
来源：http://unh.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eho.hysaishi.cn

[R16] until 等待条件
来源：http://yrw.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nim.yj20258.top

[R17] 数组定义与取值
来源：http://cvt.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fso.xylfe.cn

[R18] 遍历数组
来源：http://sgd.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ogq.ivvv.top

[R19] 数组长度
来源：http://ggc.tarul.cn

echo "${#arr[@]}"
来源：http://bgj.0kj1m.cn

[R20] 关联数组（字典）
来源：http://cql.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ptx.feifeiyinyue.top

[R21] 字符串长度
来源：http://rie.yuxming.cn

echo "${#s}"
来源：http://vtt.jinghuilouyu.cn

[R22] 截取子串
来源：http://nnm.gzhubu.top

echo "${s:0:5}"
来源：http://ptq.fktsv.cn

[R23] 字符串替换
来源：http://bso.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bsr.c1oappe.top

[R24] 大小写转换
来源：http://gvl.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://qky.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://ngx.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vnz.mhx1999.top

[R26] 命令替换
来源：http://jat.yj202588.top

now=$(date +%F); echo "$now"
来源：http://jbc.havefunace.top

[R27] 算术展开
来源：http://qmv.xuanzx.com

echo $((1 + 2 * 3))
来源：http://qci.hongshengwenyu.top

[R28] 浮点运算
来源：http://rsv.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://xla.guowangkeji.top

[R29] 定义函数
来源：http://cgp.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gwg.9152youxi.cn

[R30] 函数返回状态码
来源：http://oqf.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://evh.gogol.net.cn

[R31] 局部变量
来源：http://nie.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://cyu.shuidangran.top

[R32] 参数个数校验
来源：http://hew.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://twx.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://cfk.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://czp.epnwcf.com

[R34] 退出时清理
来源：http://qlj.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vxp.nanxuanxn.top

[R35] 后台执行并等待
来源：http://nmy.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://byx.wangdashe.top

[R36] 并发执行多个任务
来源：http://ltj.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://thp.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://mxf.hesvh.cn

files=$(ls -1)
来源：http://oqh.zhixingplan.top

[R38] 管道串联
来源：http://jsp.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://anf.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://xld.hfpthk.cn

cmd > out.log 2>&1
来源：http://hrl.shanyushiyangtech.top

[R40] 追加写日志
来源：http://wng.uphjek.com

echo "log" >> out.log
来源：http://cxk.aibaodan.cn

[R41] 丢弃输出
来源：http://tkr.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://rsf.bjfxy.top

[R42] 输入重定向
来源：http://ojq.tanke756.top

wc -l < a.txt
来源：http://snt.vehdjk.com

[R43] 按名字查找文件
来源：http://fxh.zhengqikj.top

find . -name "*.log" -type f
来源：http://ssh.gotoacloud.top

[R44] 按修改时间查找
来源：http://ssq.hesvh.cn

find . -mtime -7 -type f
来源：http://ors.wangdashe.top

[R45] 批量删除
来源：http://ppz.c1oappe.top

find . -name "*.tmp" -delete
来源：http://mcv.cashguo.top

[R46] 递归替换文件内容
来源：http://fvn.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xts.wangshuangyany.cn

[R47] sed 单行替换
来源：http://rfl.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dkg.cashguo.top

[R48] awk 取指定列
来源：http://enp.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://gta.hesvh.cn

[R49] awk 带条件
来源：http://ahx.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ayz.hysaishi.cn

[R50] awk 求和
来源：http://taw.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uxt.kuanghao11.cn

[R51] 排序去重取前几
来源：http://pvi.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bbp.iojbl.cn

[R52] 统计行数
来源：http://ldb.redwolf501.top

wc -l a.txt
来源：http://nac.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://kbe.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://odn.daxiang520.top

[R54] 比较两个文件
来源：http://zhi.shanyushiyangtech.top

diff a.txt b.txt
来源：http://ofv.ydzc1.top

[R55] 压缩与解压
来源：http://enr.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uln.meibo888.top

[R56] 远程拷贝
来源：http://qok.yangfankeji.com

scp file user@host:/path/
来源：http://vdo.guannengcc.top

[R57] 远程执行命令
来源：http://pzv.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://nld.jinqigfzy.top

[R58] 下载文件
来源：http://htu.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxa.zhongyouzk.top

[R59] 发 POST JSON
来源：http://tuk.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://avj.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://qbr.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bim.yonumen.top

[R61] 磁盘占用
来源：http://eoe.jqgufenzy.top

df -h;  du -sh *
来源：http://ckk.iojbl.cn

[R62] 找最占空间的文件
来源：http://pro.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://boe.daxiang520.top

[R63] 内存与进程
来源：http://jrj.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://hzo.haohaochexian.top

[R64] 结束进程
来源：http://rtb.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://dmv.smart0.xyz

[R65] 查看端口占用
来源：http://kyv.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://edf.52xcode.cn

[R66] 定时任务
来源：http://zte.gotoacloud.top

crontab -e;  crontab -l
来源：http://xsa.yj20258.top

[R67] 生成随机十六进制串
来源：http://luz.quarkkingdee.top

openssl rand -hex 16
来源：http://zqi.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://uyw.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://rqz.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://xar.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://gea.ppjwa.cn

[R70] 时间戳与互转
来源：http://gpe.mhx1999.top

date +%s;  date -d @1700000000
来源：http://fwh.redwolf501.top

[R71] 日期格式化
来源：http://wwk.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://xed.yj20258888.top

[R72] 等待端口就绪
来源：http://ccy.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://set.ctjpmb.com

[R73] 分割大日志
来源：http://nqf.sxryk.cn

split -l 1000 big.log part_
来源：http://ojs.gotoacloud.top

[R74] 批量重命名
来源：http://uhe.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kxv.fktsv.cn

[R75] 导出环境变量
来源：http://edu.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://mbn.jqgfzy.top

[R76] 使用临时文件
来源：http://jip.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mcm.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://jxq.nanxuanxn.top

read -rp "请输入: " ans
来源：http://ajh.cheryme.top

[R78] 交互式菜单
来源：http://doh.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zkw.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://anq.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://paa.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://xds.cdnleiting.top

time ./run.sh
来源：http://fzh.daria6918.cn

================================================================================
来源：http://rqm.zhengqikj.top


<!-- 参考信息 -->