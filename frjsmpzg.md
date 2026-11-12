代发 wailian999

[Q44] IN 子查询
来源：http://wcy.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ysh.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://vzb.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bjo.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vzh.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mab.zdbjq.cn

[Q47] 与平均值比较
来源：http://mul.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://akd.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://wpf.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aym.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://ywu.xylfe.cn

[Q49] 更新单行
来源：http://dki.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://msz.yuxming.cn

[Q50] 批量更新
来源：http://zaq.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zdt.smart0.xyz

[Q51] 用子查询更新
来源：http://kwv.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zss.snrcjt.cn

[Q52] 删除指定行
来源：http://djn.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://yoy.chenlongwang.top

[Q53] 按条件删除
来源：http://qpb.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xje.hywenlv.cn

[Q54] 清空表
来源：http://imt.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://nnf.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://ooy.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vbq.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://vxf.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://naj.guowangkeji.top

[Q57] 行号
来源：http://amu.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://icq.ydzc1.top

[Q58] 累计求和
来源：http://oor.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhh.vqdsnc.cn

[Q59] 分组内累计
来源：http://dcn.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qqg.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://fgt.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xjw.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tcw.hcnkem.com

[Q61] 移动平均
来源：http://esp.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eaw.fktsv.cn

[Q62] 分组占比
来源：http://lss.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hjm.xuanzx.com

[Q63] 开启事务
来源：http://mbw.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jiv.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://jfs.ppjwa.cn

COMMIT;
来源：http://jar.dianchejie.cn

[Q65] 回滚事务
来源：http://dne.zhaomingkeji.xyz

ROLLBACK;
来源：http://loe.chenzaomai.com

[Q66] 行锁查询
来源：http://iva.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ond.redwolf501.top

[Q67] 设置隔离级别
来源：http://wor.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zlw.jyoumei.cn

[Q68] 保存点
来源：http://aso.dashuyun.cn

SAVEPOINT sp1;
来源：http://yjt.ivvv.top

ROLLBACK TO sp1;
来源：http://mdv.jinqigufen.top

[Q69] 查看执行计划
来源：http://clj.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yrk.fehbvm.com

[Q70] 更新统计信息
来源：http://rfs.yangfankeji.com

ANALYZE TABLE users;
来源：http://zyb.haohaochexian.top

[Q71] 查看建表语句
来源：http://slz.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qms.fengsongda.top

[Q72] 查看索引
来源：http://xhd.fktsv.cn

SHOW INDEX FROM users;
来源：http://kad.yfazqb.com

[Q73] 查看表状态
来源：http://ryp.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xck.dianchejie.cn

[Q74] 强制使用索引
来源：http://kpt.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://een.gotoacloud.top

[Q75] 日期格式化
来源：http://cht.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qag.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://izz.tanke756.top

[Q76] 按天统计
来源：http://gji.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fgu.hysaishi.cn

[Q77] 时间加减
来源：http://fbt.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgt.haohaochexian.top

[Q78] 当前时间
来源：http://tge.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dos.sjlbkw.cn

[Q79] 字符串拼接
来源：http://eug.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kpc.yvedp.cn

[Q80] 字符串截取
来源：http://sbm.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oko.zdbjq.cn

[Q81] 字符串替换
来源：http://nst.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nlo.hammf.cn

[Q82] 字符长度与字节长度
来源：http://edt.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ptr.tanke756.top

[Q83] 大小写转换
来源：http://pfl.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hep.hesvh.cn

[Q84] 去除首尾空格
来源：http://yoq.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://tfl.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://klf.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ret.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://uwl.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yfa.nwbrower.top

[Q87] JSON 字段做条件
来源：http://rff.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcg.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://kpy.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jfp.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jfz.birdmap.top

[Q89] 判断表是否存在
来源：http://tvt.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iei.vehdjk.com

[Q90] 生成序号列
来源：http://sdq.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://klu.epnwcf.com

================================================================================
来源：http://roa.hnqzz.top

R. Bash 专题
来源：http://tmv.jyoumei.cn

================================================================================
来源：http://ilz.yj202588.top

[R01] shebang 与严格模式
来源：http://rug.xinyue.icu

#!/usr/bin/env bash
来源：http://wus.jinqigfzy.top

set -euo pipefail
来源：http://ycn.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://dhc.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://hvp.316326.xyz

[R03] 只读变量
来源：http://kcn.0kj1m.cn

readonly PI=3.14
来源：http://raa.sjlbkw.cn

[R04] 位置参数
来源：http://hvt.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kpp.wangshuangyany.cn

[R05] 参数默认值
来源：http://flk.yvedp.cn

name="${1:-default}"
来源：http://cnw.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://kez.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gkt.chenzaomai.com

[R07] if 判断文件
来源：http://yxr.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sef.xylfe.cn

[R08] 数值比较
来源：http://gpj.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rko.chenzaomai.com

[R09] 字符串比较
来源：http://iir.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcv.guowangkeji.top

[R10] 正则匹配
来源：http://spj.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://upk.hnxiangtu.top

[R11] case 多分支
来源：http://cay.tarul.cn

case "$1" in
来源：http://yll.yangfankeji.com

start) echo "启动" ;;
来源：http://lht.gotoacloud.top

stop)  echo "停止" ;;
来源：http://mdr.xziqi.cn

*)     echo "未知命令" ;;
来源：http://ioe.dianchejie.cn

esac
来源：http://uvn.fzhhl.top

[R12] for 遍历文件
来源：http://aof.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://okg.sxryk.cn

[R13] for 计数循环
来源：http://hgr.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://exp.xinyue.icu

[R14] C 风格 for
来源：http://gbu.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fcd.fktsv.cn

[R15] while 逐行读文件
来源：http://bpr.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pov.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://cee.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://alb.gotoacloud.top

[R17] 数组定义与取值
来源：http://pzl.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://dph.ydzc1.top

[R18] 遍历数组
来源：http://bpp.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://acf.feifeiyinyue.top

[R19] 数组长度
来源：http://bcf.tarul.cn

echo "${#arr[@]}"
来源：http://xok.hfpthk.cn

[R20] 关联数组（字典）
来源：http://npi.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vof.dianchejie.cn

[R21] 字符串长度
来源：http://bef.iojbl.cn

echo "${#s}"
来源：http://fdm.epnwcf.com

[R22] 截取子串
来源：http://rkk.xinyue.icu

echo "${s:0:5}"
来源：http://pyx.nanxuanxn.top

[R23] 字符串替换
来源：http://soo.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jgg.aizwys.cn

[R24] 大小写转换
来源：http://qfj.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://isy.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://fau.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ktg.hesvh.cn

[R26] 命令替换
来源：http://qmy.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://ktp.jqgufenzy.top

[R27] 算术展开
来源：http://xfn.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://wrv.shanyushiyangtech.top

[R28] 浮点运算
来源：http://yvr.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://gqx.gzhubu.top

[R29] 定义函数
来源：http://sau.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bet.cqqwz.cn

[R30] 函数返回状态码
来源：http://qht.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://nte.316326.xyz

[R31] 局部变量
来源：http://ffw.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://zgg.sxryk.cn

[R32] 参数个数校验
来源：http://pri.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://flx.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://gou.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqg.fktsv.cn

[R34] 退出时清理
来源：http://pqn.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://vwp.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://wiw.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yaq.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://rda.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uzo.bjfxy.top

[R37] 把输出赋给变量
来源：http://jgv.cucudq.cn

files=$(ls -1)
来源：http://lyg.cqqwz.cn

[R38] 管道串联
来源：http://mlx.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://izi.tanke756.top

[R39] 重定向标准输出与错误
来源：http://sda.0kj1m.cn

cmd > out.log 2>&1
来源：http://aka.ivvv.top

[R40] 追加写日志
来源：http://ihj.yueranfly.top

echo "log" >> out.log
来源：http://tuz.9152youxi.cn

[R41] 丢弃输出
来源：http://nel.jianghu66.top

cmd >/dev/null 2>&1
来源：http://xba.xuanzx.com

[R42] 输入重定向
来源：http://xva.jiagoushi.top

wc -l < a.txt
来源：http://yfk.jiagoushi.top

[R43] 按名字查找文件
来源：http://ffd.yj20258.top

find . -name "*.log" -type f
来源：http://pvp.nanxinkj.top

[R44] 按修改时间查找
来源：http://cho.gaohongyu789.top

find . -mtime -7 -type f
来源：http://xic.xinyue.icu

[R45] 批量删除
来源：http://dky.yuxming.cn

find . -name "*.tmp" -delete
来源：http://qhy.tianlin.xyz

[R46] 递归替换文件内容
来源：http://aad.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yry.sysykeji.top

[R47] sed 单行替换
来源：http://lcz.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mzm.yj20258.top

[R48] awk 取指定列
来源：http://nje.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://deu.gaohongyu789.top

[R49] awk 带条件
来源：http://iuo.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eos.chenjidiqi.icu

[R50] awk 求和
来源：http://svs.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ucf.pycfn.com

[R51] 排序去重取前几
来源：http://ncw.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gyz.hongshengwenyu.top

[R52] 统计行数
来源：http://vyv.nanxuanxn.top

wc -l a.txt
来源：http://jqc.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://qrg.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rtc.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://fyl.tianlin.xyz

diff a.txt b.txt
来源：http://avu.ydzc1.top

[R55] 压缩与解压
来源：http://its.c1oappe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zxd.jinqigfzy.top

[R56] 远程拷贝
来源：http://kbl.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://ncz.316326.xyz

[R57] 远程执行命令
来源：http://esw.zhixingplan.top

ssh user@host 'uptime'
来源：http://ufb.52xcode.cn

[R58] 下载文件
来源：http://sio.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://urb.jianghu66.top

[R59] 发 POST JSON
来源：http://ltb.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nue.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://kst.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lge.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://qpe.hesvh.cn

df -h;  du -sh *
来源：http://rct.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://qvx.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://jeq.mhx1999.top

[R63] 内存与进程
来源：http://dqr.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://wlb.zycfv.cn

[R64] 结束进程
来源：http://lmb.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://hel.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://ngd.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yyl.andypj.xyz

[R66] 定时任务
来源：http://bnx.uphjek.com

crontab -e;  crontab -l
来源：http://fdc.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://xlu.chenlongwang.top

openssl rand -hex 16
来源：http://pvk.pycfn.com

[R68] 计算文件校验值
来源：http://whl.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://nup.svipenyu.cn

[R69] 生成随机密码
来源：http://gfq.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://aya.zhijiandao.cn

[R70] 时间戳与互转
来源：http://jpv.tanke756.top

date +%s;  date -d @1700000000
来源：http://wvn.ybcxt.top

[R71] 日期格式化
来源：http://nbw.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://izq.tian-w.cn

[R72] 等待端口就绪
来源：http://gox.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eic.svipenyu.cn

[R73] 分割大日志
来源：http://hwu.sufxvd.cn

split -l 1000 big.log part_
来源：http://ior.birdmap.top

[R74] 批量重命名
来源：http://weo.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uks.yanxiufei.cn

[R75] 导出环境变量
来源：http://ohb.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://qox.hnxiangtu.top

[R76] 使用临时文件
来源：http://bfk.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xtf.epnwcf.com

[R77] 读取用户输入
来源：http://qsi.cqqwz.cn

read -rp "请输入: " ans
来源：http://tmc.zdqjudy.top

[R78] 交互式菜单
来源：http://gjk.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gbd.hammf.cn

[R79] 解析命令行选项
来源：http://sva.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eym.316326.xyz

[R80] 查看脚本执行耗时
来源：http://ggw.jlsjyb.cn

time ./run.sh
来源：http://zut.yj20258888.top

================================================================================
来源：http://luq.yj202588.top

S. C / C++ 专题
来源：http://myv.guannengcc.top

================================================================================
来源：http://arh.chenzaomai.com

[S01] C：Hello World
来源：http://aqv.xuetiantiany.cn

#include <stdio.h>
来源：http://ohm.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tsk.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://zmj.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://vmn.xylfe.cn

[S03] C：读入整数
来源：http://egl.xziqi.cn

int x; scanf("%d", &x);
来源：http://ois.hywenlv.cn

[S04] C：字符串复制
来源：http://dvm.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://lsx.yj202588.top

[S05] C：字符串长度
来源：http://ekq.snrcjt.cn

strlen(s)
来源：http://lee.bbcook.cn

[S06] C：字符串比较
来源：http://pzv.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://dbf.smart0.xyz

[S07] C：数组遍历求和
来源：http://rpt.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kmy.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://cqd.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ddo.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://ohw.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eul.gogol.net.cn

[S10] C：指针与解引用
来源：http://ilc.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://gqb.zhijiandao.cn

[S11] C：逐行读文件
来源：http://vor.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://yjo.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qaq.hesvh.cn

fclose(f);
来源：http://xxe.shanyushiyangkeji.top

[S12] C：写文件
来源：http://rvl.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://orn.316326.xyz

[S13] C：宏定义
来源：http://laq.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gwi.ivvv.top

[S14] C：枚举
来源：http://mdc.nwbrower.top


<!-- 参考信息 -->