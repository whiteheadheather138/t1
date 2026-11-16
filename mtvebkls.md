代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qdz.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://ece.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hei.jianghu66.top

[Q41] 多表连接
来源：http://loq.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oqi.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://rgt.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://roh.yj20258.top

[Q42] 连接条件附加过滤
来源：http://num.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://qaa.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wtb.jinqigfzy.top

[Q43] 标量子查询
来源：http://cmm.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sqy.wangdashe.top

[Q44] IN 子查询
来源：http://wsn.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://klr.316326.xyz

[Q45] EXISTS 判断存在
来源：http://sse.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://opb.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qov.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dbu.shzxlz.cn

[Q47] 与平均值比较
来源：http://rnc.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://edk.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://pnn.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jzg.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://sga.0kj1m.cn

[Q49] 更新单行
来源：http://azv.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wcc.hnxiangtu.top

[Q50] 批量更新
来源：http://gwk.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubq.wangdashe.top

[Q51] 用子查询更新
来源：http://bsd.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sjm.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://uqb.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://twf.shuidangran.top

[Q53] 按条件删除
来源：http://fgy.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tht.vqdsnc.cn

[Q54] 清空表
来源：http://noi.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://ekw.aizwys.cn

[Q55] 排名（并列占位）
来源：http://vdu.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kni.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://izr.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dwk.zhoulong.xyz

[Q57] 行号
来源：http://xht.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bgb.nanxuanxn.top

[Q58] 累计求和
来源：http://ysv.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pdn.gogol.net.cn

[Q59] 分组内累计
来源：http://zvb.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qye.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://efn.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ass.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://efm.kuanghao11.cn

[Q61] 移动平均
来源：http://dpx.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://spy.ydzc1.top

[Q62] 分组占比
来源：http://yjk.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oiq.fanxiaobao.xyz

[Q63] 开启事务
来源：http://fio.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://jns.bbcook.cn

[Q64] 提交事务
来源：http://pba.andypj.xyz

COMMIT;
来源：http://jyt.svipenyu.cn

[Q65] 回滚事务
来源：http://gqy.nanxuanxn.top

ROLLBACK;
来源：http://bwh.xinyue.icu

[Q66] 行锁查询
来源：http://eif.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fxk.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://bjd.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dao.daria6918.cn

[Q68] 保存点
来源：http://ipz.chenzaomai.com

SAVEPOINT sp1;
来源：http://jvk.haohaochexian.top

ROLLBACK TO sp1;
来源：http://ilu.fehbvm.com

[Q69] 查看执行计划
来源：http://axy.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uub.bbcook.cn

[Q70] 更新统计信息
来源：http://kue.tanke756.top

ANALYZE TABLE users;
来源：http://opq.guowangkeji.top

[Q71] 查看建表语句
来源：http://bqx.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bov.ppjwa.cn

[Q72] 查看索引
来源：http://xkd.yvedp.cn

SHOW INDEX FROM users;
来源：http://fgt.hesvh.cn

[Q73] 查看表状态
来源：http://fly.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://djm.ybcxt.top

[Q74] 强制使用索引
来源：http://utn.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rif.gaohongyu789.top

[Q75] 日期格式化
来源：http://mvh.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ltm.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://msq.guowangkeji.top

[Q76] 按天统计
来源：http://iyl.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aqx.shuidangran.top

[Q77] 时间加减
来源：http://sbv.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lup.yfazqb.com

[Q78] 当前时间
来源：http://mro.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tyr.daxiang520.top

[Q79] 字符串拼接
来源：http://zly.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hxn.tanke756.top

[Q80] 字符串截取
来源：http://blx.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sfq.dashuyun.cn

[Q81] 字符串替换
来源：http://bsy.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iui.yonumen.top

[Q82] 字符长度与字节长度
来源：http://jge.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nze.ctjpmb.com

[Q83] 大小写转换
来源：http://lnr.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wqi.yj20258.top

[Q84] 去除首尾空格
来源：http://bls.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://gwh.zhiwuduotai.top

[Q85] 数值取整
来源：http://voc.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iml.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://mcm.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tzv.yvedp.cn

[Q87] JSON 字段做条件
来源：http://tfs.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rnf.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://yxw.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qdu.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ghv.hammf.cn

[Q89] 判断表是否存在
来源：http://tew.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lni.epnwcf.com

[Q90] 生成序号列
来源：http://tqf.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ene.fehbvm.com

================================================================================
来源：http://qnm.yonumen.top

R. Bash 专题
来源：http://ztq.jinghuilouyu.cn

================================================================================
来源：http://ixu.chenlongwang.top

[R01] shebang 与严格模式
来源：http://kks.guannengcc.top

#!/usr/bin/env bash
来源：http://byu.cucudq.cn

set -euo pipefail
来源：http://ekc.cheryme.top

[R02] 变量赋值与使用
来源：http://oim.svipenyu.cn

name="Tom"; echo "$name"
来源：http://vrz.mhx1999.top

[R03] 只读变量
来源：http://eml.nanxuanxn.top

readonly PI=3.14
来源：http://agx.jlsjyb.cn

[R04] 位置参数
来源：http://tub.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ekv.dashuyun.cn

[R05] 参数默认值
来源：http://zxa.zhijiandao.cn

name="${1:-default}"
来源：http://yig.shuidangran.top

[R06] 判断命令是否存在
来源：http://hsh.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://afx.shangyingyoupin.top

[R07] if 判断文件
来源：http://yfc.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xmt.yanxiufei.cn

[R08] 数值比较
来源：http://lub.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://een.birdmap.top

[R09] 字符串比较
来源：http://zcd.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sos.fehbvm.com

[R10] 正则匹配
来源：http://rvo.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qtl.birdmap.top

[R11] case 多分支
来源：http://hax.xuanzx.com

case "$1" in
来源：http://nsx.daria6918.cn

start) echo "启动" ;;
来源：http://lxc.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://iyj.hcnkem.com

*)     echo "未知命令" ;;
来源：http://iqu.haohaochexian.top

esac
来源：http://szl.jqgufenzy.top

[R12] for 遍历文件
来源：http://rqm.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://tkl.tanke756.top

[R13] for 计数循环
来源：http://ldh.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://lnp.hfpthk.cn

[R14] C 风格 for
来源：http://rwk.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qan.iojbl.cn

[R15] while 逐行读文件
来源：http://lam.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mcu.fengsongda.top

[R16] until 等待条件
来源：http://fvy.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iin.hfpthk.cn

[R17] 数组定义与取值
来源：http://pay.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://zmr.yj20258.top

[R18] 遍历数组
来源：http://tgv.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qxx.pengpengdd.cyou

[R19] 数组长度
来源：http://bkc.mhx1999.top

echo "${#arr[@]}"
来源：http://kql.nwbrower.top

[R20] 关联数组（字典）
来源：http://glj.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svg.hongshengwenyu.top

[R21] 字符串长度
来源：http://xyp.jinghuilouyu.cn

echo "${#s}"
来源：http://zax.hfpthk.cn

[R22] 截取子串
来源：http://epg.haohaochexian.top

echo "${s:0:5}"
来源：http://cjx.sweek.top

[R23] 字符串替换
来源：http://uny.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pik.316326.xyz

[R24] 大小写转换
来源：http://ele.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://xlh.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://sjn.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://shr.chenlongwang.top

[R26] 命令替换
来源：http://kkm.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://vbf.uphjek.com

[R27] 算术展开
来源：http://vny.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://jun.fehbvm.com

[R28] 浮点运算
来源：http://mcn.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://qbc.chenlongwang.top

[R29] 定义函数
来源：http://xlt.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djb.vehdjk.com

[R30] 函数返回状态码
来源：http://imk.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://dsm.ydjk.org.cn

[R31] 局部变量
来源：http://jxt.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://kqg.zhijiandao.cn

[R32] 参数个数校验
来源：http://tsp.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgc.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://dby.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nxe.ybcxt.top

[R34] 退出时清理
来源：http://sjq.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://nmc.hesvh.cn

[R35] 后台执行并等待
来源：http://dcr.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://knl.bbcook.cn

[R36] 并发执行多个任务
来源：http://egf.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eyf.yuxming.cn

[R37] 把输出赋给变量
来源：http://qgl.hongshengwenyu.top

files=$(ls -1)
来源：http://luk.zhengqikj.top

[R38] 管道串联
来源：http://jqf.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://fjs.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://rel.tanke756.top

cmd > out.log 2>&1
来源：http://eqx.nanxuanxn.top

[R40] 追加写日志
来源：http://ddq.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://rpy.dianchejie.cn

[R41] 丢弃输出
来源：http://btm.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://obz.cdnleiting.top

[R42] 输入重定向
来源：http://fka.jinqigfzy.top

wc -l < a.txt
来源：http://ipv.wangdashe.top

[R43] 按名字查找文件
来源：http://fmf.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://ska.zycfv.cn

[R44] 按修改时间查找
来源：http://icp.cashguo.top

find . -mtime -7 -type f
来源：http://cqb.tanke756.top

[R45] 批量删除
来源：http://vjv.birdmap.top

find . -name "*.tmp" -delete
来源：http://brw.shzxlz.cn

[R46] 递归替换文件内容
来源：http://ttr.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cjg.vqdsnc.cn

[R47] sed 单行替换
来源：http://jwk.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://ltx.316326.xyz

[R48] awk 取指定列
来源：http://rbq.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://bos.0kj1m.cn

[R49] awk 带条件
来源：http://ict.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://srw.ivvv.top

[R50] awk 求和
来源：http://rpr.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://kdi.gzhubu.top

[R51] 排序去重取前几
来源：http://kpu.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://igr.gzhubu.top

[R52] 统计行数
来源：http://kdc.sufxvd.cn

wc -l a.txt
来源：http://hlh.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://cxy.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cgm.vehdjk.com

[R54] 比较两个文件
来源：http://zna.nanxinkj.top

diff a.txt b.txt
来源：http://imw.uphjek.com

[R55] 压缩与解压
来源：http://sew.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ojy.gaohongyu789.top

[R56] 远程拷贝
来源：http://wgd.aibaodan.cn

scp file user@host:/path/
来源：http://idq.quarkkingdee.top

[R57] 远程执行命令
来源：http://obz.jianghu66.top

ssh user@host 'uptime'
来源：http://dzo.shanyushiyangkeji.top

[R58] 下载文件
来源：http://apu.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ucu.nwbrower.top

[R59] 发 POST JSON
来源：http://uhu.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qgu.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://cqg.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wta.haohaochexian.top

[R61] 磁盘占用
来源：http://gaj.tarul.cn

df -h;  du -sh *
来源：http://zct.0kj1m.cn

[R62] 找最占空间的文件
来源：http://wgm.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://qni.ivvv.top

[R63] 内存与进程
来源：http://esj.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://oyc.yangfankeji.com

[R64] 结束进程
来源：http://isx.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://znr.9152youxi.cn

[R65] 查看端口占用
来源：http://bja.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yvu.ehwqpu.com

[R66] 定时任务
来源：http://pgb.ydzc1.top

crontab -e;  crontab -l
来源：http://qto.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://yig.fehbvm.com

openssl rand -hex 16
来源：http://quu.zdqjudy.top

[R68] 计算文件校验值
来源：http://bbd.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://toe.gotoacloud.top

[R69] 生成随机密码
来源：http://biv.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://wlg.xziqi.cn

[R70] 时间戳与互转
来源：http://oxv.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://kxw.andypj.xyz

[R71] 日期格式化
来源：http://qyz.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dkr.vqdsnc.cn

[R72] 等待端口就绪
来源：http://yqe.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gnr.yj202588.top

[R73] 分割大日志
来源：http://ikq.smart0.xyz

split -l 1000 big.log part_
来源：http://nai.yvedp.cn

[R74] 批量重命名
来源：http://fne.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lyy.sysykeji.top

[R75] 导出环境变量
来源：http://vwg.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://utm.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://eyy.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jpd.ydzc1.top

[R77] 读取用户输入
来源：http://tje.guannengcc.top

read -rp "请输入: " ans
来源：http://mxf.uphjek.com

[R78] 交互式菜单
来源：http://soj.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ijg.cucudq.cn

[R79] 解析命令行选项
来源：http://kum.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xvn.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://sgh.yj202588.top

time ./run.sh
来源：http://pxw.dashuyun.cn

================================================================================
来源：http://ykn.meibo888.top

S. C / C++ 专题
来源：http://lxf.pengpengdd.cyou

================================================================================
来源：http://xnn.xziqi.cn

[S01] C：Hello World
来源：http://thi.haohaochexian.top

#include <stdio.h>
来源：http://wer.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gix.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://kct.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://pat.cqqwz.cn

[S03] C：读入整数
来源：http://tfi.guannengcc.top

int x; scanf("%d", &x);
来源：http://thd.52xcode.cn

[S04] C：字符串复制
来源：http://sfg.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://fhb.fzhhl.top

[S05] C：字符串长度
来源：http://yjv.shzxlz.cn

strlen(s)
来源：http://kgt.sjlbkw.cn

[S06] C：字符串比较
来源：http://bld.ppjwa.cn

strcmp(a, b) == 0
来源：http://xzy.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://jjd.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tqi.havefunace.top

[S08] C：动态内存分配与释放
来源：http://ceq.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylv.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://tnf.ivvv.top


<!-- 参考信息 -->