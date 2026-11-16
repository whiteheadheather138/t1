代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tah.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://mzb.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://irh.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://yoj.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tsr.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://yrc.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://vvx.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://gsw.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://wgo.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bgj.yj202588.top

[Q43] 标量子查询
来源：http://bcz.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwf.xziqi.cn

[Q44] IN 子查询
来源：http://rzm.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zpa.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://htz.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://atv.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://ama.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mtx.yanxiufei.cn

[Q47] 与平均值比较
来源：http://ffd.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iry.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://wrs.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oca.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://qer.jinghuilouyu.cn

[Q49] 更新单行
来源：http://rfi.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jjr.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://hyv.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fej.xziqi.cn

[Q51] 用子查询更新
来源：http://eud.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xoh.tarul.cn

[Q52] 删除指定行
来源：http://bvr.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://sit.xinyue.icu

[Q53] 按条件删除
来源：http://tqm.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jja.snrcjt.cn

[Q54] 清空表
来源：http://cxs.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://kul.yj202588.top

[Q55] 排名（并列占位）
来源：http://mux.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xlv.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://sdv.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nvp.hywenlv.cn

[Q57] 行号
来源：http://zgj.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uej.ehwqpu.com

[Q58] 累计求和
来源：http://hlc.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ycd.zhoulong.xyz

[Q59] 分组内累计
来源：http://ucq.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sae.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://usz.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ihg.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lsx.bbcook.cn

[Q61] 移动平均
来源：http://xnx.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ikp.sxryk.cn

[Q62] 分组占比
来源：http://cpm.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zoo.dianchejie.cn

[Q63] 开启事务
来源：http://mdn.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dog.andypj.xyz

[Q64] 提交事务
来源：http://gzs.aizwys.cn

COMMIT;
来源：http://cwc.gaohongyu789.top

[Q65] 回滚事务
来源：http://lft.yangfankeji.com

ROLLBACK;
来源：http://ptz.hammf.cn

[Q66] 行锁查询
来源：http://xnb.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vgb.zdbjq.cn

[Q67] 设置隔离级别
来源：http://ecm.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://too.zhixingplan.top

[Q68] 保存点
来源：http://ybs.hnxiangtu.top

SAVEPOINT sp1;
来源：http://clq.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://kya.guowangkeji.top

[Q69] 查看执行计划
来源：http://mjn.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jhu.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://pzg.ctjpmb.com

ANALYZE TABLE users;
来源：http://whk.meibo888.top

[Q71] 查看建表语句
来源：http://ksd.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qux.hywenlv.cn

[Q72] 查看索引
来源：http://pzj.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://lbc.shangyingyoupin.top

[Q73] 查看表状态
来源：http://niw.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://deg.chenzaomai.com

[Q74] 强制使用索引
来源：http://baf.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pun.fehbvm.com

[Q75] 日期格式化
来源：http://rdp.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dac.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://svb.sufxvd.cn

[Q76] 按天统计
来源：http://ics.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bub.bbcook.cn

[Q77] 时间加减
来源：http://mms.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gqr.jqgfzy.top

[Q78] 当前时间
来源：http://bdv.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jem.gzhubu.top

[Q79] 字符串拼接
来源：http://pnx.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bou.havefunace.top

[Q80] 字符串截取
来源：http://eju.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovf.yj202588.top

[Q81] 字符串替换
来源：http://jsz.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ngp.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://ebs.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tyw.yueranfly.top

[Q83] 大小写转换
来源：http://tgd.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wae.mhx1999.top

[Q84] 去除首尾空格
来源：http://tzq.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://wxr.tian-w.cn

[Q85] 数值取整
来源：http://gsl.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vml.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://chy.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://udw.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://uom.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nlm.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://ijh.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bzj.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fly.hysaishi.cn

[Q89] 判断表是否存在
来源：http://luf.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lak.zhongyouzk.top

[Q90] 生成序号列
来源：http://axa.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ciq.wangdashe.top

================================================================================
来源：http://jsp.dianchejie.cn

R. Bash 专题
来源：http://wfa.daxiang520.top

================================================================================
来源：http://fma.52xcode.cn

[R01] shebang 与严格模式
来源：http://fvh.sweek.top

#!/usr/bin/env bash
来源：http://mkn.jinyuanbaomall.cn

set -euo pipefail
来源：http://fxv.sweek.top

[R02] 变量赋值与使用
来源：http://bxq.zhixingplan.top

name="Tom"; echo "$name"
来源：http://jgr.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://lyu.kuanghao11.cn

readonly PI=3.14
来源：http://plo.jianghu66.top

[R04] 位置参数
来源：http://jcz.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://emr.zhijiandao.cn

[R05] 参数默认值
来源：http://elh.cashguo.top

name="${1:-default}"
来源：http://hba.yvedp.cn

[R06] 判断命令是否存在
来源：http://vgj.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://upm.hammf.cn

[R07] if 判断文件
来源：http://zvv.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cly.sysykeji.top

[R08] 数值比较
来源：http://tmz.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vzn.zhijiandao.cn

[R09] 字符串比较
来源：http://hpa.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cxn.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://cru.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iys.uphjek.com

[R11] case 多分支
来源：http://zjd.sxryk.cn

case "$1" in
来源：http://ysg.yuanzhike.top

start) echo "启动" ;;
来源：http://lbl.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://bhx.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://lri.gaohongyu789.top

esac
来源：http://wkh.shuidangran.top

[R12] for 遍历文件
来源：http://qah.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://zag.andypj.xyz

[R13] for 计数循环
来源：http://uuw.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://znb.gotoacloud.top

[R14] C 风格 for
来源：http://pkk.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ngi.sufxvd.cn

[R15] while 逐行读文件
来源：http://whd.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ant.jianghu66.top

[R16] until 等待条件
来源：http://qvy.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oua.zhoulong.xyz

[R17] 数组定义与取值
来源：http://ype.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://xdc.fanxiaobao.xyz

[R18] 遍历数组
来源：http://ofb.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sve.gaohongyu789.top

[R19] 数组长度
来源：http://bjj.hysaishi.cn

echo "${#arr[@]}"
来源：http://fyv.aizwys.cn

[R20] 关联数组（字典）
来源：http://lux.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zil.chenzaomai.com

[R21] 字符串长度
来源：http://izl.zhijiandao.cn

echo "${#s}"
来源：http://ayu.gzhubu.top

[R22] 截取子串
来源：http://dbp.nanxinkj.top

echo "${s:0:5}"
来源：http://dtw.yuxming.cn

[R23] 字符串替换
来源：http://leq.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ior.fzhhl.top

[R24] 大小写转换
来源：http://zzn.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://ulm.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://qjy.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ilc.havefunace.top

[R26] 命令替换
来源：http://kth.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://bwr.ppjwa.cn

[R27] 算术展开
来源：http://rjm.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://cpp.jyoumei.cn

[R28] 浮点运算
来源：http://ojf.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://prd.yueranfly.top

[R29] 定义函数
来源：http://zkk.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sqp.iojbl.cn

[R30] 函数返回状态码
来源：http://cxc.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://had.cashguo.top

[R31] 局部变量
来源：http://xbw.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://jzd.gzhubu.top

[R32] 参数个数校验
来源：http://huk.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://afo.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://zmk.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xtf.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://qai.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kry.uphjek.com

[R35] 后台执行并等待
来源：http://owl.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://khl.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://pil.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://epl.meibo888.top

[R37] 把输出赋给变量
来源：http://ewc.yangfankeji.com

files=$(ls -1)
来源：http://qko.daria6918.cn

[R38] 管道串联
来源：http://cdi.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://hiv.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://jkt.0kj1m.cn

cmd > out.log 2>&1
来源：http://nzs.bbcook.cn

[R40] 追加写日志
来源：http://ziy.52xcode.cn

echo "log" >> out.log
来源：http://vtk.birdmap.top

[R41] 丢弃输出
来源：http://xva.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://upq.sxryk.cn

[R42] 输入重定向
来源：http://duy.wangdashe.top

wc -l < a.txt
来源：http://wfk.zhongyouzk.top

[R43] 按名字查找文件
来源：http://drt.tian-w.cn

find . -name "*.log" -type f
来源：http://sfi.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://egt.haohaochexian.top

find . -mtime -7 -type f
来源：http://cka.52xcode.cn

[R45] 批量删除
来源：http://wjv.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://abf.gzhubu.top

[R46] 递归替换文件内容
来源：http://cxt.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lbi.0kj1m.cn

[R47] sed 单行替换
来源：http://ipd.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://dgl.ivvv.top

[R48] awk 取指定列
来源：http://qrw.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://yyr.yonumen.top

[R49] awk 带条件
来源：http://dcv.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uyw.aibaodan.cn

[R50] awk 求和
来源：http://mhd.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://zkd.yvedp.cn

[R51] 排序去重取前几
来源：http://nox.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://teh.jinyuanbaomall.cn

[R52] 统计行数
来源：http://zyu.wangshuangyany.cn

wc -l a.txt
来源：http://qqb.316326.xyz

[R53] 查看文件头与实时尾
来源：http://cpz.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://spm.hcnkem.com

[R54] 比较两个文件
来源：http://zwu.hesvh.cn

diff a.txt b.txt
来源：http://blk.zdqjudy.top

[R55] 压缩与解压
来源：http://abb.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xwx.havefunace.top

[R56] 远程拷贝
来源：http://rfw.tarul.cn

scp file user@host:/path/
来源：http://qyt.yfazqb.com

[R57] 远程执行命令
来源：http://ppz.bjfxy.top

ssh user@host 'uptime'
来源：http://ccm.ywan-chungtsiang.top

[R58] 下载文件
来源：http://lsa.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rnz.yvedp.cn

[R59] 发 POST JSON
来源：http://srq.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxl.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://zuu.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gys.shuidangran.top

[R61] 磁盘占用
来源：http://hhb.zhengqikj.top

df -h;  du -sh *
来源：http://enh.hcnkem.com

[R62] 找最占空间的文件
来源：http://pbm.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://nhp.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://adg.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://sjq.zycfv.cn

[R64] 结束进程
来源：http://nhz.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://nqi.pengpengdd.cyou

[R65] 查看端口占用
来源：http://vum.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hmz.jqgfzy.top

[R66] 定时任务
来源：http://drt.zdbjq.cn

crontab -e;  crontab -l
来源：http://jjn.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://jsh.daria6918.cn

openssl rand -hex 16
来源：http://lfa.xinyue.icu

[R68] 计算文件校验值
来源：http://pnl.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jsp.bjfxy.top

[R69] 生成随机密码
来源：http://lom.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://jfl.ydjk.org.cn

[R70] 时间戳与互转
来源：http://nbt.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://frd.zdqjudy.top

[R71] 日期格式化
来源：http://hfk.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yec.smart0.xyz

[R72] 等待端口就绪
来源：http://ptg.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vjj.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://euo.hnqzz.top

split -l 1000 big.log part_
来源：http://wls.cdnleiting.top

[R74] 批量重命名
来源：http://lqi.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jsh.ydzc1.top

[R75] 导出环境变量
来源：http://rth.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://ccf.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://xnk.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kph.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://ulc.zycfv.cn

read -rp "请输入: " ans
来源：http://fvy.zhijiandao.cn

[R78] 交互式菜单
来源：http://yll.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qzl.meibo888.top

[R79] 解析命令行选项
来源：http://rgy.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mdy.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://opk.chenlongwang.top

time ./run.sh
来源：http://itf.cdnleiting.top

================================================================================
来源：http://wog.fzhhl.top

S. C / C++ 专题
来源：http://tho.zycfv.cn

================================================================================
来源：http://hsa.dashuyun.cn

[S01] C：Hello World
来源：http://ubs.mhx1999.top

#include <stdio.h>
来源：http://zts.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://djg.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://nmu.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://gob.fanxiaobao.xyz

[S03] C：读入整数
来源：http://dvj.fengsongda.top

int x; scanf("%d", &x);
来源：http://vca.hnxiangtu.top

[S04] C：字符串复制
来源：http://xre.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://pyw.daxiang520.top

[S05] C：字符串长度
来源：http://wja.hcnkem.com

strlen(s)
来源：http://lwo.tanke756.top

[S06] C：字符串比较
来源：http://agr.zhixingplan.top

strcmp(a, b) == 0
来源：http://fhq.chenzaomai.com

[S07] C：数组遍历求和
来源：http://iih.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://opt.tanke756.top

[S08] C：动态内存分配与释放
来源：http://hxd.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vvl.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://cyq.fzhhl.top


<!-- 参考信息 -->