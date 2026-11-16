代发 wailian999

[Q48] CTE 公用表表达式
来源：http://rbg.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjd.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://kaf.haohaochexian.top

[Q49] 更新单行
来源：http://lgv.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hsb.xinyue.icu

[Q50] 批量更新
来源：http://djb.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uxt.cheryme.top

[Q51] 用子查询更新
来源：http://nfv.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hcz.hesvh.cn

[Q52] 删除指定行
来源：http://gxs.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://ooi.svipenyu.cn

[Q53] 按条件删除
来源：http://yzx.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://myk.nanxinkj.top

[Q54] 清空表
来源：http://gxq.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://uwb.yj20258.top

[Q55] 排名（并列占位）
来源：http://rhx.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rxr.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://jki.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xws.zhiwuduotai.top

[Q57] 行号
来源：http://afq.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cho.smart0.xyz

[Q58] 累计求和
来源：http://clp.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uvm.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://ryg.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rgj.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://pnd.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://paf.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xnb.xylfe.cn

[Q61] 移动平均
来源：http://cvn.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ivz.yueranfly.top

[Q62] 分组占比
来源：http://iwk.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jzm.sysykeji.top

[Q63] 开启事务
来源：http://qya.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zey.fengsongda.top

[Q64] 提交事务
来源：http://fhl.meibo888.top

COMMIT;
来源：http://aws.zhiwuduotai.top

[Q65] 回滚事务
来源：http://xjy.wangshuangyany.cn

ROLLBACK;
来源：http://tty.bjfxy.top

[Q66] 行锁查询
来源：http://opg.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qnh.yfazqb.com

[Q67] 设置隔离级别
来源：http://den.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ezt.nanxinkj.top

[Q68] 保存点
来源：http://fci.zhijiandao.cn

SAVEPOINT sp1;
来源：http://qtm.gzhubu.top

ROLLBACK TO sp1;
来源：http://twd.yanxiufei.cn

[Q69] 查看执行计划
来源：http://oso.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axb.zdqjudy.top

[Q70] 更新统计信息
来源：http://sug.hysaishi.cn

ANALYZE TABLE users;
来源：http://ize.guannengcc.top

[Q71] 查看建表语句
来源：http://hng.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pmt.52xcode.cn

[Q72] 查看索引
来源：http://dft.jiagoushi.top

SHOW INDEX FROM users;
来源：http://emv.quarkkingdee.top

[Q73] 查看表状态
来源：http://zpo.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eqc.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://jyh.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qnb.wangdashe.top

[Q75] 日期格式化
来源：http://dcf.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lrc.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qgt.smart0.xyz

[Q76] 按天统计
来源：http://ymy.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uag.wangshuangyany.cn

[Q77] 时间加减
来源：http://bdb.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cyp.fengsongda.top

[Q78] 当前时间
来源：http://zis.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://brz.ivvv.top

[Q79] 字符串拼接
来源：http://ljz.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eml.zhengqikj.top

[Q80] 字符串截取
来源：http://gdo.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://htd.xziqi.cn

[Q81] 字符串替换
来源：http://nve.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wtg.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://igs.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xdr.jqgfzy.top

[Q83] 大小写转换
来源：http://hem.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmp.bjfxy.top

[Q84] 去除首尾空格
来源：http://pwk.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://nya.redwolf501.top

[Q85] 数值取整
来源：http://oss.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://slk.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://qne.gzhubu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nyl.sxryk.cn

[Q87] JSON 字段做条件
来源：http://kfu.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fjm.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://wpy.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mlu.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zss.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://xnb.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pcb.zdqjudy.top

[Q90] 生成序号列
来源：http://dzu.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vnl.snrcjt.cn

================================================================================
来源：http://fmr.hysaishi.cn

R. Bash 专题
来源：http://ijr.jyoumei.cn

================================================================================
来源：http://zrs.zycfv.cn

[R01] shebang 与严格模式
来源：http://pde.iojbl.cn

#!/usr/bin/env bash
来源：http://uvp.guannengcc.top

set -euo pipefail
来源：http://bvh.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://mqy.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://zjm.316326.xyz

[R03] 只读变量
来源：http://uyb.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://ril.vqdsnc.cn

[R04] 位置参数
来源：http://ezl.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sac.zhongyouzk.top

[R05] 参数默认值
来源：http://hkk.jinqigfzy.top

name="${1:-default}"
来源：http://wyh.cdnleiting.top

[R06] 判断命令是否存在
来源：http://qcw.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fbu.cucudq.cn

[R07] if 判断文件
来源：http://unh.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ckh.aibaodan.cn

[R08] 数值比较
来源：http://aja.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ttt.vehdjk.com

[R09] 字符串比较
来源：http://djb.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fen.gaohongyu789.top

[R10] 正则匹配
来源：http://eue.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yvk.zdbjq.cn

[R11] case 多分支
来源：http://jlm.yanxiufei.cn

case "$1" in
来源：http://nqj.fzhhl.top

start) echo "启动" ;;
来源：http://opi.andypj.xyz

stop)  echo "停止" ;;
来源：http://jjl.yj202588.top

*)     echo "未知命令" ;;
来源：http://drx.hesvh.cn

esac
来源：http://yal.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://bnd.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://rgh.fengsongda.top

[R13] for 计数循环
来源：http://rga.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://gae.yvedp.cn

[R14] C 风格 for
来源：http://xxb.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hcj.yj20258888.top

[R15] while 逐行读文件
来源：http://ljn.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jlo.fzhhl.top

[R16] until 等待条件
来源：http://nji.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sqa.meibo888.top

[R17] 数组定义与取值
来源：http://bws.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://caf.hcnkem.com

[R18] 遍历数组
来源：http://wbl.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yjk.daxiang520.top

[R19] 数组长度
来源：http://ccr.chenzaomai.com

echo "${#arr[@]}"
来源：http://wgr.vehdjk.com

[R20] 关联数组（字典）
来源：http://uda.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aah.fzhhl.top

[R21] 字符串长度
来源：http://fka.fktsv.cn

echo "${#s}"
来源：http://qqj.ivvv.top

[R22] 截取子串
来源：http://ldq.bbcook.cn

echo "${s:0:5}"
来源：http://dgu.cashguo.top

[R23] 字符串替换
来源：http://lxb.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rit.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://ejr.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://fxe.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://geu.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ryv.shangyingyoupin.top

[R26] 命令替换
来源：http://zff.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://yqi.tanke756.top

[R27] 算术展开
来源：http://wcm.c1oappe.top

echo $((1 + 2 * 3))
来源：http://nat.gzhubu.top

[R28] 浮点运算
来源：http://jgl.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://ulm.ydzc1.top

[R29] 定义函数
来源：http://bko.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iop.jqgufenzy.top

[R30] 函数返回状态码
来源：http://zay.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://iwd.nanxinkj.top

[R31] 局部变量
来源：http://loj.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://zqa.316326.xyz

[R32] 参数个数校验
来源：http://rfq.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nxu.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://bdx.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rlf.guannengcc.top

[R34] 退出时清理
来源：http://pwx.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://zmi.yanxiufei.cn

[R35] 后台执行并等待
来源：http://ilw.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mvf.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://wlk.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unu.fehbvm.com

[R37] 把输出赋给变量
来源：http://pns.aibaodan.cn

files=$(ls -1)
来源：http://ylq.hnxiangtu.top

[R38] 管道串联
来源：http://sph.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://oib.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://pvk.epnwcf.com

cmd > out.log 2>&1
来源：http://mqq.tianlin.xyz

[R40] 追加写日志
来源：http://fjy.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://eti.pengpengdd.cyou

[R41] 丢弃输出
来源：http://ily.sweek.top

cmd >/dev/null 2>&1
来源：http://lfq.dianchejie.cn

[R42] 输入重定向
来源：http://hyv.wangshuangyany.cn

wc -l < a.txt
来源：http://nhl.guowangkeji.top

[R43] 按名字查找文件
来源：http://lat.fehbvm.com

find . -name "*.log" -type f
来源：http://xde.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://elp.sxryk.cn

find . -mtime -7 -type f
来源：http://ydr.sweek.top

[R45] 批量删除
来源：http://fpg.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://pxt.gzhubu.top

[R46] 递归替换文件内容
来源：http://omc.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uir.snrcjt.cn

[R47] sed 单行替换
来源：http://vqv.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gwz.wangdashe.top

[R48] awk 取指定列
来源：http://qgy.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://qkj.316326.xyz

[R49] awk 带条件
来源：http://mjm.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pwn.cheryme.top

[R50] awk 求和
来源：http://dma.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://ugu.vehdjk.com

[R51] 排序去重取前几
来源：http://dyw.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://chy.c1oappe.top

[R52] 统计行数
来源：http://xbe.zhixingplan.top

wc -l a.txt
来源：http://lfd.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://usn.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jhy.zycfv.cn

[R54] 比较两个文件
来源：http://mfw.ydjk.org.cn

diff a.txt b.txt
来源：http://tzn.vqdsnc.cn

[R55] 压缩与解压
来源：http://jkp.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ahr.yuxming.cn

[R56] 远程拷贝
来源：http://lbv.meibo888.top

scp file user@host:/path/
来源：http://sgs.cheryme.top

[R57] 远程执行命令
来源：http://boh.yfazqb.com

ssh user@host 'uptime'
来源：http://mtk.cucudq.cn

[R58] 下载文件
来源：http://mim.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aks.xylfe.cn

[R59] 发 POST JSON
来源：http://zmk.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ljk.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://tob.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fee.feifeiyinyue.top

[R61] 磁盘占用
来源：http://vqn.wangdashe.top

df -h;  du -sh *
来源：http://ibk.gzhubu.top

[R62] 找最占空间的文件
来源：http://oyw.yonumen.top

du -ah . | sort -rh | head -10
来源：http://qym.zhongyouzk.top

[R63] 内存与进程
来源：http://inr.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://poq.zhengqikj.top

[R64] 结束进程
来源：http://csr.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://yvb.jyoumei.cn

[R65] 查看端口占用
来源：http://yhd.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rqf.sweek.top

[R66] 定时任务
来源：http://mco.hcnkem.com

crontab -e;  crontab -l
来源：http://gfp.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://fxj.chenzaomai.com

openssl rand -hex 16
来源：http://lgy.tanke756.top

[R68] 计算文件校验值
来源：http://laa.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://tzx.zhixingplan.top

[R69] 生成随机密码
来源：http://jxh.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://uig.pycfn.com

[R70] 时间戳与互转
来源：http://few.zycfv.cn

date +%s;  date -d @1700000000
来源：http://tbs.hesvh.cn

[R71] 日期格式化
来源：http://wrt.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dqq.52xcode.cn

[R72] 等待端口就绪
来源：http://fbm.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://wve.ivvv.top

[R73] 分割大日志
来源：http://lto.yj20258.top

split -l 1000 big.log part_
来源：http://myt.tanke756.top

[R74] 批量重命名
来源：http://yvf.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uym.yj20258.top

[R75] 导出环境变量
来源：http://mne.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://joz.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://uch.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ykv.c1oappe.top

[R77] 读取用户输入
来源：http://eay.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://sar.yangfankeji.com

[R78] 交互式菜单
来源：http://tul.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kvm.zhijiandao.cn

[R79] 解析命令行选项
来源：http://mao.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://slc.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://gyh.hysaishi.cn

time ./run.sh
来源：http://fsq.yuxming.cn

================================================================================
来源：http://yua.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://eim.chenzaomai.com

================================================================================
来源：http://bwu.havefunace.top

[S01] C：Hello World
来源：http://brh.zhaomingkeji.xyz

#include <stdio.h>
来源：http://rtt.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bvt.meibo888.top

[S02] C：变量与格式化输出
来源：http://roi.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://lzd.zdqjudy.top

[S03] C：读入整数
来源：http://opw.fengsongda.top

int x; scanf("%d", &x);
来源：http://ckd.aibaodan.cn

[S04] C：字符串复制
来源：http://vqd.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dsi.zycfv.cn

[S05] C：字符串长度
来源：http://xou.jinghuilouyu.cn

strlen(s)
来源：http://osa.zhengqikj.top

[S06] C：字符串比较
来源：http://plv.hnxiangtu.top

strcmp(a, b) == 0
来源：http://rxz.ctjpmb.com

[S07] C：数组遍历求和
来源：http://yvr.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xdt.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://rxd.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://emw.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://vin.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ksd.sxryk.cn

[S10] C：指针与解引用
来源：http://ant.daxiang520.top

int *p = &a;  *p = 5;
来源：http://xgu.bbcook.cn

[S11] C：逐行读文件
来源：http://phe.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://pbm.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iyd.jqgufenzy.top

fclose(f);
来源：http://qme.dashuyun.cn

[S12] C：写文件
来源：http://xpb.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://emq.fzhhl.top

[S13] C：宏定义
来源：http://omp.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lsr.sxryk.cn

[S14] C：枚举
来源：http://eni.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zyp.tarul.cn

[S15] C：类型转换
来源：http://acn.yfazqb.com

(double) a / b
来源：http://ceg.yj20258888.top

[S16] C：位操作置位
来源：http://tay.kuanghao11.cn

x |= (1 << 3);
来源：http://ptk.shuidangran.top

[S17] C：安全拼接字符串
来源：http://obc.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yxl.kuanghao11.cn

[S18] C：命令行参数
来源：http://zwn.daxiang520.top


<!-- 参考信息 -->