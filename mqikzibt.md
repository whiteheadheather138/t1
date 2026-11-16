代发 wailian999

[Q44] IN 子查询
来源：http://xes.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nua.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://tvh.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sbl.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://frp.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvv.cdnleiting.top

[Q47] 与平均值比较
来源：http://mhp.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://trn.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://fku.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rkx.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://okk.wangdashe.top

[Q49] 更新单行
来源：http://ihm.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qsx.yj20258.top

[Q50] 批量更新
来源：http://oeg.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://urb.meibo888.top

[Q51] 用子查询更新
来源：http://dcf.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yun.mhx1999.top

[Q52] 删除指定行
来源：http://ibx.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://ren.xylfe.cn

[Q53] 按条件删除
来源：http://cyh.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://isq.hnxiangtu.top

[Q54] 清空表
来源：http://ply.fktsv.cn

TRUNCATE TABLE logs;
来源：http://fva.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://mne.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rvt.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://xmz.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qec.zhoulong.xyz

[Q57] 行号
来源：http://mdr.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bht.andypj.xyz

[Q58] 累计求和
来源：http://onm.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wwn.fzhhl.top

[Q59] 分组内累计
来源：http://pzf.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pib.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://dfc.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://enj.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qki.pengpengdd.cyou

[Q61] 移动平均
来源：http://uqw.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wgn.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://kqq.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qdc.chenlongwang.top

[Q63] 开启事务
来源：http://efe.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://twq.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://wiv.redwolf501.top

COMMIT;
来源：http://bab.chenzaomai.com

[Q65] 回滚事务
来源：http://pzj.shanyushiyangtech.top

ROLLBACK;
来源：http://hcq.jqgfzy.top

[Q66] 行锁查询
来源：http://cal.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cyp.bjfxy.top

[Q67] 设置隔离级别
来源：http://foc.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bdo.chenzaomai.com

[Q68] 保存点
来源：http://ffx.hnxiangtu.top

SAVEPOINT sp1;
来源：http://yqg.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://lao.mhx1999.top

[Q69] 查看执行计划
来源：http://soo.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ich.tarul.cn

[Q70] 更新统计信息
来源：http://lsk.zhijiandao.cn

ANALYZE TABLE users;
来源：http://rck.hysaishi.cn

[Q71] 查看建表语句
来源：http://wxs.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zmm.xziqi.cn

[Q72] 查看索引
来源：http://imh.sweek.top

SHOW INDEX FROM users;
来源：http://uur.ybcxt.top

[Q73] 查看表状态
来源：http://wpe.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oro.tanke756.top

[Q74] 强制使用索引
来源：http://tjv.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://klz.fktsv.cn

[Q75] 日期格式化
来源：http://xei.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hgq.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ync.feifeiyinyue.top

[Q76] 按天统计
来源：http://rgj.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tlm.yj202588.top

[Q77] 时间加减
来源：http://kmt.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ais.yj20258888.top

[Q78] 当前时间
来源：http://pue.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uoj.ydzc1.top

[Q79] 字符串拼接
来源：http://zpp.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tdo.gzhubu.top

[Q80] 字符串截取
来源：http://vad.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://usf.shzxlz.cn

[Q81] 字符串替换
来源：http://zjo.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sir.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://xme.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fnn.ydjk.org.cn

[Q83] 大小写转换
来源：http://jjq.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gyc.0kj1m.cn

[Q84] 去除首尾空格
来源：http://fii.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://ago.fanxiaobao.xyz

[Q85] 数值取整
来源：http://mvy.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dto.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://yll.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ykf.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://alf.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dii.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://oxz.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xzc.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjl.tarul.cn

[Q89] 判断表是否存在
来源：http://qtp.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iez.yfazqb.com

[Q90] 生成序号列
来源：http://nmz.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ajz.guowangkeji.top

================================================================================
来源：http://qkl.cheryme.top

R. Bash 专题
来源：http://bna.sjlbkw.cn

================================================================================
来源：http://ael.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://cuo.fzhhl.top

#!/usr/bin/env bash
来源：http://ens.shanyushiyangkeji.top

set -euo pipefail
来源：http://rbz.bbcook.cn

[R02] 变量赋值与使用
来源：http://fss.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://pxq.birdmap.top

[R03] 只读变量
来源：http://sgv.sxryk.cn

readonly PI=3.14
来源：http://pvd.yj202588.top

[R04] 位置参数
来源：http://gpy.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ifx.jiagoushi.top

[R05] 参数默认值
来源：http://gfy.jianghu66.top

name="${1:-default}"
来源：http://tjc.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://smb.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tom.xuanzx.com

[R07] if 判断文件
来源：http://cnd.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://akf.yongpay.top

[R08] 数值比较
来源：http://see.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vha.hongshengwenyu.top

[R09] 字符串比较
来源：http://bcs.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mte.yanxiufei.cn

[R10] 正则匹配
来源：http://lxs.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bhw.xuanzx.com

[R11] case 多分支
来源：http://amn.chenjidiqi.icu

case "$1" in
来源：http://azf.jqgfzy.top

start) echo "启动" ;;
来源：http://quk.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://lzl.tanke756.top

*)     echo "未知命令" ;;
来源：http://kyd.sxryk.cn

esac
来源：http://hlm.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://yoi.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://uwz.redwolf501.top

[R13] for 计数循环
来源：http://hty.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://wrp.tianlin.xyz

[R14] C 风格 for
来源：http://mjv.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cxi.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://ypy.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lzd.ctjpmb.com

[R16] until 等待条件
来源：http://twj.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zju.ctjpmb.com

[R17] 数组定义与取值
来源：http://nuh.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://kci.yongpay.top

[R18] 遍历数组
来源：http://mhq.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ydb.ehwqpu.com

[R19] 数组长度
来源：http://tnc.jinqigufen.top

echo "${#arr[@]}"
来源：http://jib.hammf.cn

[R20] 关联数组（字典）
来源：http://xkd.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wnv.chenlongwang.top

[R21] 字符串长度
来源：http://iva.tarul.cn

echo "${#s}"
来源：http://nio.wangshuangyany.cn

[R22] 截取子串
来源：http://mll.9152youxi.cn

echo "${s:0:5}"
来源：http://ucn.meibo888.top

[R23] 字符串替换
来源：http://rjw.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://swe.xylfe.cn

[R24] 大小写转换
来源：http://fgt.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://ijb.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://iwm.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lni.zhiwuduotai.top

[R26] 命令替换
来源：http://nvd.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://qbi.jyoumei.cn

[R27] 算术展开
来源：http://nax.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://wql.cdnleiting.top

[R28] 浮点运算
来源：http://ffz.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://ega.epnwcf.com

[R29] 定义函数
来源：http://xvi.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vvy.jqgufenzy.top

[R30] 函数返回状态码
来源：http://mkj.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://pio.tanke756.top

[R31] 局部变量
来源：http://skr.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://qmi.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://vtl.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://och.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://wih.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bvg.hcnkem.com

[R34] 退出时清理
来源：http://cah.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vex.52xcode.cn

[R35] 后台执行并等待
来源：http://zxf.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ffd.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://ufq.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gvy.gzhubu.top

[R37] 把输出赋给变量
来源：http://eqt.shuidangran.top

files=$(ls -1)
来源：http://ntx.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://oae.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://fgt.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://kve.tanke756.top

cmd > out.log 2>&1
来源：http://jbp.zhoulong.xyz

[R40] 追加写日志
来源：http://oor.chenlongwang.top

echo "log" >> out.log
来源：http://pre.sxryk.cn

[R41] 丢弃输出
来源：http://yhf.redwolf501.top

cmd >/dev/null 2>&1
来源：http://usj.nanxuanxn.top

[R42] 输入重定向
来源：http://fhn.sweek.top

wc -l < a.txt
来源：http://gzx.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://vwf.jiagoushi.top

find . -name "*.log" -type f
来源：http://iiu.dianchejie.cn

[R44] 按修改时间查找
来源：http://mdd.mhx1999.top

find . -mtime -7 -type f
来源：http://jcs.dashuyun.cn

[R45] 批量删除
来源：http://nde.havefunace.top

find . -name "*.tmp" -delete
来源：http://dyi.yuanzhike.top

[R46] 递归替换文件内容
来源：http://xzh.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dhk.tanke756.top

[R47] sed 单行替换
来源：http://hkd.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://umf.havefunace.top

[R48] awk 取指定列
来源：http://him.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://rqz.vqdsnc.cn

[R49] awk 带条件
来源：http://nif.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oww.ydjk.org.cn

[R50] awk 求和
来源：http://hde.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vkm.cashguo.top

[R51] 排序去重取前几
来源：http://bly.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vkx.quarkkingdee.top

[R52] 统计行数
来源：http://xwg.gzhubu.top

wc -l a.txt
来源：http://qen.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://gvl.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://faa.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://bbx.smart0.xyz

diff a.txt b.txt
来源：http://lto.9152youxi.cn

[R55] 压缩与解压
来源：http://mlp.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idi.daxiang520.top

[R56] 远程拷贝
来源：http://zdz.sysykeji.top

scp file user@host:/path/
来源：http://gtu.ehwqpu.com

[R57] 远程执行命令
来源：http://ohj.guowangkeji.top

ssh user@host 'uptime'
来源：http://dmh.yongpay.top

[R58] 下载文件
来源：http://wgs.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ypa.ehwqpu.com

[R59] 发 POST JSON
来源：http://nha.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bhd.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://bru.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xyg.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://yyi.sysykeji.top

df -h;  du -sh *
来源：http://voj.hammf.cn

[R62] 找最占空间的文件
来源：http://mbo.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://rjg.jinghuilouyu.cn

[R63] 内存与进程
来源：http://zqm.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://wty.xuanzx.com

[R64] 结束进程
来源：http://tlu.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://ogp.ybcxt.top

[R65] 查看端口占用
来源：http://gxy.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bzo.hnqzz.top

[R66] 定时任务
来源：http://gtg.hcnkem.com

crontab -e;  crontab -l
来源：http://qap.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://crj.sxryk.cn

openssl rand -hex 16
来源：http://hyo.cdnleiting.top

[R68] 计算文件校验值
来源：http://vfj.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://twe.dianchejie.cn

[R69] 生成随机密码
来源：http://uiy.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://jak.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://zch.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://qiy.shzxlz.cn

[R71] 日期格式化
来源：http://iwo.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsb.hnxiangtu.top

[R72] 等待端口就绪
来源：http://fvt.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ngu.jiagoushi.top

[R73] 分割大日志
来源：http://ech.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://vpi.shanyushiyangtech.top

[R74] 批量重命名
来源：http://hns.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gkj.andypj.xyz

[R75] 导出环境变量
来源：http://gti.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://yzm.fktsv.cn

[R76] 使用临时文件
来源：http://krl.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://equ.c1oappe.top

[R77] 读取用户输入
来源：http://aht.jinqigufen.top

read -rp "请输入: " ans
来源：http://xme.9152youxi.cn

[R78] 交互式菜单
来源：http://lnk.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qxm.zhoulong.xyz

[R79] 解析命令行选项
来源：http://fnl.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ayh.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://qgc.yuxming.cn

time ./run.sh
来源：http://imz.chenjidiqi.icu

================================================================================
来源：http://eil.daria6918.cn

S. C / C++ 专题
来源：http://ort.ydjk.org.cn

================================================================================
来源：http://izu.uphjek.com

[S01] C：Hello World
来源：http://rrf.zdqjudy.top

#include <stdio.h>
来源：http://ndy.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ccr.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://qpq.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://mtm.zhongyouzk.top

[S03] C：读入整数
来源：http://gvf.vehdjk.com

int x; scanf("%d", &x);
来源：http://ykr.hfpthk.cn

[S04] C：字符串复制
来源：http://kqc.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jvi.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://lyp.iojbl.cn

strlen(s)
来源：http://ucc.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://baj.zhongyouzk.top

strcmp(a, b) == 0
来源：http://xck.yonumen.top

[S07] C：数组遍历求和
来源：http://vqr.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jyd.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://inz.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xlq.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://hhi.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ycy.ehwqpu.com

[S10] C：指针与解引用
来源：http://elq.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://dpx.tianlin.xyz

[S11] C：逐行读文件
来源：http://wih.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://fpy.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zfr.zhaomingkeji.xyz

fclose(f);
来源：http://mki.ivvv.top

[S12] C：写文件
来源：http://ayk.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ymt.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://gmj.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yhl.sxryk.cn

[S14] C：枚举
来源：http://uik.hnqzz.top


<!-- 参考信息 -->