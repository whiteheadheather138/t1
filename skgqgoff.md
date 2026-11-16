代发 wailian999

[Q48] CTE 公用表表达式
来源：http://sqo.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://txr.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://lnu.zhongyouzk.top

[Q49] 更新单行
来源：http://nwd.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gkq.fzhhl.top

[Q50] 批量更新
来源：http://yzn.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tfj.jqgfzy.top

[Q51] 用子查询更新
来源：http://zih.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fif.gotoacloud.top

[Q52] 删除指定行
来源：http://sed.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://bqh.zhengqikj.top

[Q53] 按条件删除
来源：http://iss.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dda.kuanghao11.cn

[Q54] 清空表
来源：http://zag.fktsv.cn

TRUNCATE TABLE logs;
来源：http://ldw.hammf.cn

[Q55] 排名（并列占位）
来源：http://kwm.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lxr.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://elf.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://exu.nanxinkj.top

[Q57] 行号
来源：http://mza.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bqb.zhoulong.xyz

[Q58] 累计求和
来源：http://hqd.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gdz.ctjpmb.com

[Q59] 分组内累计
来源：http://jxk.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fjy.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://khl.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://knq.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dbl.daria6918.cn

[Q61] 移动平均
来源：http://wya.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hmp.gzhubu.top

[Q62] 分组占比
来源：http://jcm.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://riy.daria6918.cn

[Q63] 开启事务
来源：http://jgb.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hkk.tian-w.cn

[Q64] 提交事务
来源：http://ehu.daxiang520.top

COMMIT;
来源：http://ace.tianlin.xyz

[Q65] 回滚事务
来源：http://mvs.tanke756.top

ROLLBACK;
来源：http://asd.chenlongwang.top

[Q66] 行锁查询
来源：http://icw.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wua.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://dno.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cuc.sysykeji.top

[Q68] 保存点
来源：http://svu.sxryk.cn

SAVEPOINT sp1;
来源：http://hhp.gogol.net.cn

ROLLBACK TO sp1;
来源：http://bwf.xylfe.cn

[Q69] 查看执行计划
来源：http://cst.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iim.zhengqikj.top

[Q70] 更新统计信息
来源：http://ojy.ppjwa.cn

ANALYZE TABLE users;
来源：http://tma.yj20258.top

[Q71] 查看建表语句
来源：http://wag.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wqo.jiagoushi.top

[Q72] 查看索引
来源：http://zjx.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://yoj.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://zud.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mpq.nanxinkj.top

[Q74] 强制使用索引
来源：http://ucy.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hge.hcnkem.com

[Q75] 日期格式化
来源：http://wky.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wot.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dxf.hesvh.cn

[Q76] 按天统计
来源：http://drd.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ini.bjfxy.top

[Q77] 时间加减
来源：http://gdk.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fok.jianghu66.top

[Q78] 当前时间
来源：http://ekr.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uvg.0kj1m.cn

[Q79] 字符串拼接
来源：http://yaf.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rwf.gogol.net.cn

[Q80] 字符串截取
来源：http://bmm.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aoc.yj202588.top

[Q81] 字符串替换
来源：http://djy.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fpx.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://dsp.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqh.ppjwa.cn

[Q83] 大小写转换
来源：http://zyc.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ysn.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://luv.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://nxp.nanxuanxn.top

[Q85] 数值取整
来源：http://vnw.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://llf.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://sdz.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://san.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://frj.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cso.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://iyv.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ykh.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qdq.yj20258888.top

[Q89] 判断表是否存在
来源：http://ovm.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jhe.birdmap.top

[Q90] 生成序号列
来源：http://ing.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://res.cashguo.top

================================================================================
来源：http://mss.jiagoushi.top

R. Bash 专题
来源：http://ozg.yj20258888.top

================================================================================
来源：http://wxa.yongpay.top

[R01] shebang 与严格模式
来源：http://wua.yj20258888.top

#!/usr/bin/env bash
来源：http://afv.zdbjq.cn

set -euo pipefail
来源：http://qdc.316326.xyz

[R02] 变量赋值与使用
来源：http://meh.jqgfzy.top

name="Tom"; echo "$name"
来源：http://tgc.mhx1999.top

[R03] 只读变量
来源：http://ksq.jinqigfzy.top

readonly PI=3.14
来源：http://siy.cheryme.top

[R04] 位置参数
来源：http://nop.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wym.shanyushiyangtech.top

[R05] 参数默认值
来源：http://mku.tanke756.top

name="${1:-default}"
来源：http://oes.daxiang520.top

[R06] 判断命令是否存在
来源：http://wmt.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uii.ivvv.top

[R07] if 判断文件
来源：http://bfz.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bfh.ydjk.org.cn

[R08] 数值比较
来源：http://ken.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://hfm.cashguo.top

[R09] 字符串比较
来源：http://rok.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gez.sxryk.cn

[R10] 正则匹配
来源：http://dlv.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sck.chenzaomai.com

[R11] case 多分支
来源：http://rgs.yuanzhike.top

case "$1" in
来源：http://muo.nwbrower.top

start) echo "启动" ;;
来源：http://zba.52xcode.cn

stop)  echo "停止" ;;
来源：http://nfj.sysykeji.top

*)     echo "未知命令" ;;
来源：http://nqg.nwbrower.top

esac
来源：http://kac.nanxuanxn.top

[R12] for 遍历文件
来源：http://etr.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://xjw.sweek.top

[R13] for 计数循环
来源：http://ghi.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://acx.guowangkeji.top

[R14] C 风格 for
来源：http://mag.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jnn.andypj.xyz

[R15] while 逐行读文件
来源：http://aej.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uvp.hfpthk.cn

[R16] until 等待条件
来源：http://rtt.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gur.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://qgj.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://mla.guannengcc.top

[R18] 遍历数组
来源：http://zdi.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emq.hnxiangtu.top

[R19] 数组长度
来源：http://xcp.jinqigufen.top

echo "${#arr[@]}"
来源：http://qen.cdnleiting.top

[R20] 关联数组（字典）
来源：http://fqy.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ttm.hongshengwenyu.top

[R21] 字符串长度
来源：http://xma.yangfankeji.com

echo "${#s}"
来源：http://dck.zhixingplan.top

[R22] 截取子串
来源：http://asv.9152youxi.cn

echo "${s:0:5}"
来源：http://zhf.yj20258888.top

[R23] 字符串替换
来源：http://zgo.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lhs.sufxvd.cn

[R24] 大小写转换
来源：http://ojf.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://doj.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://exp.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tzr.tian-w.cn

[R26] 命令替换
来源：http://ykm.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://iel.hnxiangtu.top

[R27] 算术展开
来源：http://epv.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://ipp.wangshuangyany.cn

[R28] 浮点运算
来源：http://djc.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://iek.iojbl.cn

[R29] 定义函数
来源：http://jzi.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://huw.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://pkk.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://xvl.52xcode.cn

[R31] 局部变量
来源：http://gkp.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://flz.nanxuanxn.top

[R32] 参数个数校验
来源：http://hhr.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sar.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://hxu.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ozs.guannengcc.top

[R34] 退出时清理
来源：http://uyd.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wnm.guannengcc.top

[R35] 后台执行并等待
来源：http://pbw.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://spe.yongpay.top

[R36] 并发执行多个任务
来源：http://fzj.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nyx.ivvv.top

[R37] 把输出赋给变量
来源：http://igo.0kj1m.cn

files=$(ls -1)
来源：http://hob.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://rik.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://ipx.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://aid.jianghu66.top

cmd > out.log 2>&1
来源：http://fpv.xuanzx.com

[R40] 追加写日志
来源：http://xro.vehdjk.com

echo "log" >> out.log
来源：http://ryb.hfpthk.cn

[R41] 丢弃输出
来源：http://wht.tarul.cn

cmd >/dev/null 2>&1
来源：http://slt.kuanghao11.cn

[R42] 输入重定向
来源：http://ozv.feifeiyinyue.top

wc -l < a.txt
来源：http://elg.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://fjc.0kj1m.cn

find . -name "*.log" -type f
来源：http://iij.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://mlb.cdnleiting.top

find . -mtime -7 -type f
来源：http://ntj.zycfv.cn

[R45] 批量删除
来源：http://rhx.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://vbj.xziqi.cn

[R46] 递归替换文件内容
来源：http://mex.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://etl.xuetiantiany.cn

[R47] sed 单行替换
来源：http://suy.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dtu.snrcjt.cn

[R48] awk 取指定列
来源：http://hxe.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://prw.nanxinkj.top

[R49] awk 带条件
来源：http://rlj.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dzn.pengpengdd.cyou

[R50] awk 求和
来源：http://qkb.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tpn.sysykeji.top

[R51] 排序去重取前几
来源：http://pgj.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hkh.yuxming.cn

[R52] 统计行数
来源：http://qdq.ywan-chungtsiang.top

wc -l a.txt
来源：http://edz.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://uht.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykn.chenlongwang.top

[R54] 比较两个文件
来源：http://sir.feifeiyinyue.top

diff a.txt b.txt
来源：http://bbm.bbcook.cn

[R55] 压缩与解压
来源：http://jjj.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zrl.wangdashe.top

[R56] 远程拷贝
来源：http://wfu.ctjpmb.com

scp file user@host:/path/
来源：http://zrq.fzhhl.top

[R57] 远程执行命令
来源：http://elw.zhoulong.xyz

ssh user@host 'uptime'
来源：http://hdz.zdbjq.cn

[R58] 下载文件
来源：http://txc.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yvk.quarkkingdee.top

[R59] 发 POST JSON
来源：http://nha.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ihm.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://lug.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://one.sysykeji.top

[R61] 磁盘占用
来源：http://ybo.tarul.cn

df -h;  du -sh *
来源：http://gca.zdqjudy.top

[R62] 找最占空间的文件
来源：http://fic.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://mpm.yvedp.cn

[R63] 内存与进程
来源：http://bhk.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://ckc.gogol.net.cn

[R64] 结束进程
来源：http://amj.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://yfw.sjlbkw.cn

[R65] 查看端口占用
来源：http://lxi.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://npy.sxryk.cn

[R66] 定时任务
来源：http://mvf.hnqzz.top

crontab -e;  crontab -l
来源：http://bdg.smart0.xyz

[R67] 生成随机十六进制串
来源：http://saa.hnxiangtu.top

openssl rand -hex 16
来源：http://fqh.zhoulong.xyz

[R68] 计算文件校验值
来源：http://yix.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://crz.xuetiantiany.cn

[R69] 生成随机密码
来源：http://ilg.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://mep.wangdashe.top

[R70] 时间戳与互转
来源：http://pkd.smart0.xyz

date +%s;  date -d @1700000000
来源：http://loq.yongpay.top

[R71] 日期格式化
来源：http://tpn.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://opr.xuanzx.com

[R72] 等待端口就绪
来源：http://jwt.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://luy.andypj.xyz

[R73] 分割大日志
来源：http://lbq.iojbl.cn

split -l 1000 big.log part_
来源：http://hmk.dianchejie.cn

[R74] 批量重命名
来源：http://afm.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vme.dianchejie.cn

[R75] 导出环境变量
来源：http://tvn.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://kwe.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://inh.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oct.daxiang520.top

[R77] 读取用户输入
来源：http://cyn.tian-w.cn

read -rp "请输入: " ans
来源：http://qiu.52xcode.cn

[R78] 交互式菜单
来源：http://uya.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jkb.zhongyouzk.top

[R79] 解析命令行选项
来源：http://ses.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jff.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://epj.bjfxy.top

time ./run.sh
来源：http://zwa.gaohongyu789.top

================================================================================
来源：http://aym.tian-w.cn

S. C / C++ 专题
来源：http://odk.daria6918.cn

================================================================================
来源：http://xdz.hnqzz.top

[S01] C：Hello World
来源：http://bpi.dashuyun.cn

#include <stdio.h>
来源：http://ewn.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhh.nwbrower.top

[S02] C：变量与格式化输出
来源：http://bsu.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://tfp.sxryk.cn

[S03] C：读入整数
来源：http://pls.jiagoushi.top

int x; scanf("%d", &x);
来源：http://vfv.fengsongda.top

[S04] C：字符串复制
来源：http://meq.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://zpn.ydjk.org.cn

[S05] C：字符串长度
来源：http://kkl.tianlin.xyz

strlen(s)
来源：http://qgm.jiagoushi.top

[S06] C：字符串比较
来源：http://uax.shzxlz.cn

strcmp(a, b) == 0
来源：http://cym.xinyue.icu

[S07] C：数组遍历求和
来源：http://fce.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kzj.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://scf.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://efs.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://tne.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lmd.yonumen.top

[S10] C：指针与解引用
来源：http://yed.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://zan.yangfankeji.com

[S11] C：逐行读文件
来源：http://dsm.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://kfx.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://huj.cheryme.top

fclose(f);
来源：http://wjr.52xcode.cn

[S12] C：写文件
来源：http://ytd.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iwq.zdbjq.cn

[S13] C：宏定义
来源：http://eob.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ana.zhijiandao.cn

[S14] C：枚举
来源：http://ipe.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://hks.ehwqpu.com

[S15] C：类型转换
来源：http://rqb.dianchejie.cn

(double) a / b
来源：http://phx.nanxuanxn.top

[S16] C：位操作置位
来源：http://ygk.xuetiantiany.cn

x |= (1 << 3);
来源：http://fry.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://fqh.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://spl.nanxinkj.top

[S18] C：命令行参数
来源：http://wdt.yuxming.cn


<!-- 参考信息 -->