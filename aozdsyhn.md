代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ahd.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://hqy.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vlh.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dfx.cheryme.top

[Q61] 移动平均
来源：http://upf.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mps.meibo888.top

[Q62] 分组占比
来源：http://mhh.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ozu.cucudq.cn

[Q63] 开启事务
来源：http://mkl.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rpd.hnqzz.top

[Q64] 提交事务
来源：http://nrb.nanxinkj.top

COMMIT;
来源：http://qqn.nanxuanxn.top

[Q65] 回滚事务
来源：http://hxs.tian-w.cn

ROLLBACK;
来源：http://lny.yfazqb.com

[Q66] 行锁查询
来源：http://iov.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lgg.zdbjq.cn

[Q67] 设置隔离级别
来源：http://rlk.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jpj.zhaomingkeji.xyz

[Q68] 保存点
来源：http://fgt.epnwcf.com

SAVEPOINT sp1;
来源：http://qtv.sweek.top

ROLLBACK TO sp1;
来源：http://hvp.vehdjk.com

[Q69] 查看执行计划
来源：http://jyw.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aca.hammf.cn

[Q70] 更新统计信息
来源：http://dso.zhongyouzk.top

ANALYZE TABLE users;
来源：http://abm.ppjwa.cn

[Q71] 查看建表语句
来源：http://pov.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ywe.gaohongyu789.top

[Q72] 查看索引
来源：http://eln.52xcode.cn

SHOW INDEX FROM users;
来源：http://krn.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://tkt.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://gwr.gaohongyu789.top

[Q74] 强制使用索引
来源：http://qaf.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://daj.birdmap.top

[Q75] 日期格式化
来源：http://dzh.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gsy.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eni.meibo888.top

[Q76] 按天统计
来源：http://zpx.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ezv.hywenlv.cn

[Q77] 时间加减
来源：http://yzv.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ewb.hywenlv.cn

[Q78] 当前时间
来源：http://lfp.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mgc.haohaochexian.top

[Q79] 字符串拼接
来源：http://ven.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vmx.yangfankeji.com

[Q80] 字符串截取
来源：http://pfd.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ipx.cashguo.top

[Q81] 字符串替换
来源：http://kwe.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qnm.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://nxl.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ogr.birdmap.top

[Q83] 大小写转换
来源：http://bkh.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tsx.bbcook.cn

[Q84] 去除首尾空格
来源：http://aca.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://knj.yueranfly.top

[Q85] 数值取整
来源：http://sqw.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nfc.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://rwp.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cfz.guannengcc.top

[Q87] JSON 字段做条件
来源：http://nhf.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ync.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://ofr.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lbq.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zru.hfpthk.cn

[Q89] 判断表是否存在
来源：http://djk.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zub.yvedp.cn

[Q90] 生成序号列
来源：http://ksh.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qnl.nwbrower.top

================================================================================
来源：http://qyb.redwolf501.top

R. Bash 专题
来源：http://crv.yj20258.top

================================================================================
来源：http://jbf.fengsongda.top

[R01] shebang 与严格模式
来源：http://rqb.jqgufenzy.top

#!/usr/bin/env bash
来源：http://dei.ywan-chungtsiang.top

set -euo pipefail
来源：http://skr.yuxming.cn

[R02] 变量赋值与使用
来源：http://vnf.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://vae.nanxuanxn.top

[R03] 只读变量
来源：http://eqs.haohaochexian.top

readonly PI=3.14
来源：http://tgw.yvedp.cn

[R04] 位置参数
来源：http://keb.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eut.shuidangran.top

[R05] 参数默认值
来源：http://kam.gzhubu.top

name="${1:-default}"
来源：http://hew.jianghu66.top

[R06] 判断命令是否存在
来源：http://pmr.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pdo.ppjwa.cn

[R07] if 判断文件
来源：http://rmc.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xrs.aibaodan.cn

[R08] 数值比较
来源：http://nli.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://igz.jqgfzy.top

[R09] 字符串比较
来源：http://cvx.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tql.zdbjq.cn

[R10] 正则匹配
来源：http://uqo.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ukh.hysaishi.cn

[R11] case 多分支
来源：http://wdq.haohaochexian.top

case "$1" in
来源：http://zdy.yueranfly.top

start) echo "启动" ;;
来源：http://gve.redwolf501.top

stop)  echo "停止" ;;
来源：http://kzy.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://jat.fanxiaobao.xyz

esac
来源：http://vfr.jianghu66.top

[R12] for 遍历文件
来源：http://gbj.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://dkv.yonumen.top

[R13] for 计数循环
来源：http://qsm.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vjt.shuidangran.top

[R14] C 风格 for
来源：http://lhj.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gqm.zhengqikj.top

[R15] while 逐行读文件
来源：http://ymb.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uxc.tanke756.top

[R16] until 等待条件
来源：http://pht.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uoz.sysykeji.top

[R17] 数组定义与取值
来源：http://xrb.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bxx.feifeiyinyue.top

[R18] 遍历数组
来源：http://fvm.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ive.ppjwa.cn

[R19] 数组长度
来源：http://syp.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://hjk.ybcxt.top

[R20] 关联数组（字典）
来源：http://ctp.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yge.xziqi.cn

[R21] 字符串长度
来源：http://jpc.hongshengwenyu.top

echo "${#s}"
来源：http://qbj.haohaochexian.top

[R22] 截取子串
来源：http://ftz.hysaishi.cn

echo "${s:0:5}"
来源：http://aqc.redwolf501.top

[R23] 字符串替换
来源：http://mgm.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlf.hywenlv.cn

[R24] 大小写转换
来源：http://hlo.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://djp.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://mng.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibn.yfazqb.com

[R26] 命令替换
来源：http://oqm.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://chj.dianchejie.cn

[R27] 算术展开
来源：http://yte.birdmap.top

echo $((1 + 2 * 3))
来源：http://xzf.epnwcf.com

[R28] 浮点运算
来源：http://ghe.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://wjz.shanyushiyangtech.top

[R29] 定义函数
来源：http://lfn.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://klk.andypj.xyz

[R30] 函数返回状态码
来源：http://hmg.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://gss.wangdashe.top

[R31] 局部变量
来源：http://ubd.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://mlv.havefunace.top

[R32] 参数个数校验
来源：http://juz.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zvh.316326.xyz

[R33] 捕获错误并提示行号
来源：http://whw.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xrw.cashguo.top

[R34] 退出时清理
来源：http://yli.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://snu.shzxlz.cn

[R35] 后台执行并等待
来源：http://tdo.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://rxe.zhengqikj.top

[R36] 并发执行多个任务
来源：http://pke.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfz.yvedp.cn

[R37] 把输出赋给变量
来源：http://mdp.hnqzz.top

files=$(ls -1)
来源：http://bfa.redwolf501.top

[R38] 管道串联
来源：http://nxa.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://ona.hammf.cn

[R39] 重定向标准输出与错误
来源：http://ftm.zhengqikj.top

cmd > out.log 2>&1
来源：http://gwp.xziqi.cn

[R40] 追加写日志
来源：http://con.jiagoushi.top

echo "log" >> out.log
来源：http://hyu.smart0.xyz

[R41] 丢弃输出
来源：http://xuk.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://fdh.gotoacloud.top

[R42] 输入重定向
来源：http://wyd.sufxvd.cn

wc -l < a.txt
来源：http://tbh.aizwys.cn

[R43] 按名字查找文件
来源：http://mij.jiagoushi.top

find . -name "*.log" -type f
来源：http://ljx.aizwys.cn

[R44] 按修改时间查找
来源：http://cwc.dianchejie.cn

find . -mtime -7 -type f
来源：http://bje.cashguo.top

[R45] 批量删除
来源：http://zvp.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://djk.wangdashe.top

[R46] 递归替换文件内容
来源：http://raz.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lie.xinyue.icu

[R47] sed 单行替换
来源：http://wib.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dzk.ehwqpu.com

[R48] awk 取指定列
来源：http://yxi.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://uws.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://hil.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yrj.svipenyu.cn

[R50] awk 求和
来源：http://tjs.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://hwy.gzhubu.top

[R51] 排序去重取前几
来源：http://pcf.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kip.sjlbkw.cn

[R52] 统计行数
来源：http://adb.yongpay.top

wc -l a.txt
来源：http://ujp.birdmap.top

[R53] 查看文件头与实时尾
来源：http://gie.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ogl.nanxinkj.top

[R54] 比较两个文件
来源：http://erf.fehbvm.com

diff a.txt b.txt
来源：http://rgx.pycfn.com

[R55] 压缩与解压
来源：http://eog.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dfh.zhoulong.xyz

[R56] 远程拷贝
来源：http://tnq.zhongyouzk.top

scp file user@host:/path/
来源：http://ivy.aizwys.cn

[R57] 远程执行命令
来源：http://lpq.shzxlz.cn

ssh user@host 'uptime'
来源：http://lol.xuetiantiany.cn

[R58] 下载文件
来源：http://xvx.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fts.yueranfly.top

[R59] 发 POST JSON
来源：http://syg.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zze.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://gfi.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zyz.iojbl.cn

[R61] 磁盘占用
来源：http://vwf.daxiang520.top

df -h;  du -sh *
来源：http://zzv.chenzaomai.com

[R62] 找最占空间的文件
来源：http://zbo.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://taa.tianlin.xyz

[R63] 内存与进程
来源：http://sco.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://twi.fktsv.cn

[R64] 结束进程
来源：http://qdt.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://tmz.shuidangran.top

[R65] 查看端口占用
来源：http://csj.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bvh.ehwqpu.com

[R66] 定时任务
来源：http://sag.xziqi.cn

crontab -e;  crontab -l
来源：http://ngq.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://zlk.yuanzhike.top

openssl rand -hex 16
来源：http://kjp.yangfankeji.com

[R68] 计算文件校验值
来源：http://wyz.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://swn.jiagoushi.top

[R69] 生成随机密码
来源：http://vmm.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ejm.chenlongwang.top

[R70] 时间戳与互转
来源：http://kbh.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://yjy.cheryme.top

[R71] 日期格式化
来源：http://yhx.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://skq.ybcxt.top

[R72] 等待端口就绪
来源：http://ict.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sho.c1oappe.top

[R73] 分割大日志
来源：http://wnz.yj202588.top

split -l 1000 big.log part_
来源：http://jgm.ydzc1.top

[R74] 批量重命名
来源：http://bks.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ntb.hnqzz.top

[R75] 导出环境变量
来源：http://ciw.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://xny.yfazqb.com

[R76] 使用临时文件
来源：http://jqj.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dtu.hammf.cn

[R77] 读取用户输入
来源：http://vqm.hnxiangtu.top

read -rp "请输入: " ans
来源：http://pyb.316326.xyz

[R78] 交互式菜单
来源：http://avg.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pzg.hesvh.cn

[R79] 解析命令行选项
来源：http://vqi.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://omr.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://eqf.fzhhl.top

time ./run.sh
来源：http://xwp.iojbl.cn

================================================================================
来源：http://xbo.yuxming.cn

S. C / C++ 专题
来源：http://hxa.ywan-chungtsiang.top

================================================================================
来源：http://nmj.fktsv.cn

[S01] C：Hello World
来源：http://vxd.nanxuanxn.top

#include <stdio.h>
来源：http://djz.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://juk.xuanzx.com

[S02] C：变量与格式化输出
来源：http://dks.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://jno.hcnkem.com

[S03] C：读入整数
来源：http://drx.cashguo.top

int x; scanf("%d", &x);
来源：http://zsr.shangyingyoupin.top

[S04] C：字符串复制
来源：http://ubz.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dgy.tanke756.top

[S05] C：字符串长度
来源：http://znz.chenjidiqi.icu

strlen(s)
来源：http://gbc.hesvh.cn

[S06] C：字符串比较
来源：http://ccb.sufxvd.cn

strcmp(a, b) == 0
来源：http://uzz.dashuyun.cn

[S07] C：数组遍历求和
来源：http://gvk.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://evc.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://sqx.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://puu.pycfn.com

[S09] C：结构体定义与初始化
来源：http://kml.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tkr.zhijiandao.cn

[S10] C：指针与解引用
来源：http://ojt.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://opf.iojbl.cn

[S11] C：逐行读文件
来源：http://uht.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://yyf.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://frx.xziqi.cn

fclose(f);
来源：http://cui.xylfe.cn

[S12] C：写文件
来源：http://azp.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ygo.aibaodan.cn

[S13] C：宏定义
来源：http://vub.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://amk.meibo888.top

[S14] C：枚举
来源：http://iqo.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://xdc.xuetiantiany.cn

[S15] C：类型转换
来源：http://ihe.jinyuanbaomall.cn

(double) a / b
来源：http://pdm.ybcxt.top

[S16] C：位操作置位
来源：http://eup.sxryk.cn

x |= (1 << 3);
来源：http://siu.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://vpl.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vxp.gzhubu.top

[S18] C：命令行参数
来源：http://oqb.vehdjk.com

int main(int argc, char **argv)
来源：http://mbw.ydzc1.top

[S19] C：快速排序
来源：http://igm.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xtx.xuetiantiany.cn

[S20] C：二分查找
来源：http://rrd.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kni.zhengqikj.top

[S21] C：字符类别判断
来源：http://twl.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fka.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://mrl.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://grz.sufxvd.cn

[S23] C：随机数
来源：http://tgy.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dsc.cqqwz.cn

[S24] C：获取本地时间
来源：http://bfj.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pmw.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://zxm.aibaodan.cn

memcpy(dst, src, n);
来源：http://alz.smart0.xyz

[S26] C：内存清零
来源：http://fjc.redwolf501.top

memset(a, 0, sizeof a);
来源：http://hvo.ydzc1.top

[S27] C：定义常量
来源：http://abo.wangdashe.top

const double PI = 3.14159;
来源：http://lhv.ydzc1.top

[S28] C：静态变量
来源：http://cml.xinyue.icu

static int counter = 0;
来源：http://kdi.xziqi.cn

[S29] C：变参函数
来源：http://fbs.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aho.hysaishi.cn

[S30] C：头文件保护
来源：http://rkd.jiagoushi.top


<!-- 参考信息 -->