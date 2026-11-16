代发 wailian999

[Q61] 移动平均
来源：http://ibc.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oyv.fengsongda.top

[Q62] 分组占比
来源：http://pxb.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://alq.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://zmr.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vlu.sweek.top

[Q64] 提交事务
来源：http://bpo.vehdjk.com

COMMIT;
来源：http://hrm.snrcjt.cn

[Q65] 回滚事务
来源：http://rkq.fanxiaobao.xyz

ROLLBACK;
来源：http://leb.ivvv.top

[Q66] 行锁查询
来源：http://zyh.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wcz.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://jcm.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vcf.jianghu66.top

[Q68] 保存点
来源：http://njj.ybcxt.top

SAVEPOINT sp1;
来源：http://lir.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://rer.iojbl.cn

[Q69] 查看执行计划
来源：http://cdh.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sry.cqqwz.cn

[Q70] 更新统计信息
来源：http://poy.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://tbz.pycfn.com

[Q71] 查看建表语句
来源：http://owg.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nqt.hysaishi.cn

[Q72] 查看索引
来源：http://phz.chenlongwang.top

SHOW INDEX FROM users;
来源：http://unu.birdmap.top

[Q73] 查看表状态
来源：http://cby.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uqq.daxiang520.top

[Q74] 强制使用索引
来源：http://pqk.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nyi.yongpay.top

[Q75] 日期格式化
来源：http://ndm.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://irg.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gtx.bbcook.cn

[Q76] 按天统计
来源：http://iif.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cba.jiagoushi.top

[Q77] 时间加减
来源：http://lxb.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aiw.yangfankeji.com

[Q78] 当前时间
来源：http://oih.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://syz.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://cez.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bjm.hysaishi.cn

[Q80] 字符串截取
来源：http://gpu.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xpb.jqgufenzy.top

[Q81] 字符串替换
来源：http://nmx.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jvc.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://tyl.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ksb.haohaochexian.top

[Q83] 大小写转换
来源：http://stm.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozw.0kj1m.cn

[Q84] 去除首尾空格
来源：http://vxl.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://cjl.dashuyun.cn

[Q85] 数值取整
来源：http://xdf.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://onr.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://okz.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gky.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://soi.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tfa.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://jfc.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://efq.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ocr.daxiang520.top

[Q89] 判断表是否存在
来源：http://bph.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bhp.jinqigufen.top

[Q90] 生成序号列
来源：http://mdh.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pqy.pycfn.com

================================================================================
来源：http://adw.sufxvd.cn

R. Bash 专题
来源：http://rsc.gaohongyu789.top

================================================================================
来源：http://jhm.andypj.xyz

[R01] shebang 与严格模式
来源：http://kbr.vqdsnc.cn

#!/usr/bin/env bash
来源：http://aej.52xcode.cn

set -euo pipefail
来源：http://sdb.cdnleiting.top

[R02] 变量赋值与使用
来源：http://sdx.chenlongwang.top

name="Tom"; echo "$name"
来源：http://mvd.cucudq.cn

[R03] 只读变量
来源：http://neh.xuanzx.com

readonly PI=3.14
来源：http://qeg.yfazqb.com

[R04] 位置参数
来源：http://gnx.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ran.yvedp.cn

[R05] 参数默认值
来源：http://nym.pengpengdd.cyou

name="${1:-default}"
来源：http://fku.chenlongwang.top

[R06] 判断命令是否存在
来源：http://exu.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qxg.316326.xyz

[R07] if 判断文件
来源：http://yoz.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ogt.jianghu66.top

[R08] 数值比较
来源：http://mpa.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zav.ivvv.top

[R09] 字符串比较
来源：http://qgp.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jte.0kj1m.cn

[R10] 正则匹配
来源：http://ceg.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mva.yueranfly.top

[R11] case 多分支
来源：http://atf.kuanghao11.cn

case "$1" in
来源：http://ynu.redwolf501.top

start) echo "启动" ;;
来源：http://bec.sweek.top

stop)  echo "停止" ;;
来源：http://yrj.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://aka.iojbl.cn

esac
来源：http://cfk.wangdashe.top

[R12] for 遍历文件
来源：http://mla.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://euv.jqgufenzy.top

[R13] for 计数循环
来源：http://vyq.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://gmd.dianchejie.cn

[R14] C 风格 for
来源：http://ivm.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mmg.zdqjudy.top

[R15] while 逐行读文件
来源：http://dql.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kze.zhongyouzk.top

[R16] until 等待条件
来源：http://sga.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nej.zycfv.cn

[R17] 数组定义与取值
来源：http://uix.hfpthk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rab.dashuyun.cn

[R18] 遍历数组
来源：http://ryn.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sts.0kj1m.cn

[R19] 数组长度
来源：http://eyt.9152youxi.cn

echo "${#arr[@]}"
来源：http://jdo.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://fex.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gaq.xinyue.icu

[R21] 字符串长度
来源：http://rzk.zhongyouzk.top

echo "${#s}"
来源：http://xwe.yj20258888.top

[R22] 截取子串
来源：http://uby.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://dnq.hfpthk.cn

[R23] 字符串替换
来源：http://jbh.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eoz.gzhubu.top

[R24] 大小写转换
来源：http://obq.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://aip.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://xgs.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wlf.hfpthk.cn

[R26] 命令替换
来源：http://lcs.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://ugz.aibaodan.cn

[R27] 算术展开
来源：http://vex.fengsongda.top

echo $((1 + 2 * 3))
来源：http://jiv.bbcook.cn

[R28] 浮点运算
来源：http://ygv.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://rcl.316326.xyz

[R29] 定义函数
来源：http://nep.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wyj.tarul.cn

[R30] 函数返回状态码
来源：http://yjx.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://mmg.hnxiangtu.top

[R31] 局部变量
来源：http://nws.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://puf.redwolf501.top

[R32] 参数个数校验
来源：http://bbm.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://njw.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://ipk.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nff.52xcode.cn

[R34] 退出时清理
来源：http://hht.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://alt.gogol.net.cn

[R35] 后台执行并等待
来源：http://ssq.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zuh.guannengcc.top

[R36] 并发执行多个任务
来源：http://bfc.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fmk.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://eac.ywan-chungtsiang.top

files=$(ls -1)
来源：http://otw.cdnleiting.top

[R38] 管道串联
来源：http://byl.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://goy.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://ovs.wangdashe.top

cmd > out.log 2>&1
来源：http://jwo.tarul.cn

[R40] 追加写日志
来源：http://gic.wangshuangyany.cn

echo "log" >> out.log
来源：http://nyf.hnxiangtu.top

[R41] 丢弃输出
来源：http://orn.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://pcq.quarkkingdee.top

[R42] 输入重定向
来源：http://lnp.cucudq.cn

wc -l < a.txt
来源：http://npp.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://gdv.zycfv.cn

find . -name "*.log" -type f
来源：http://few.daria6918.cn

[R44] 按修改时间查找
来源：http://jac.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://civ.ydzc1.top

[R45] 批量删除
来源：http://ksc.ydzc1.top

find . -name "*.tmp" -delete
来源：http://jhf.hywenlv.cn

[R46] 递归替换文件内容
来源：http://esy.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqe.jianghu66.top

[R47] sed 单行替换
来源：http://lel.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://ydm.zhongyouzk.top

[R48] awk 取指定列
来源：http://grl.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://gmy.yvedp.cn

[R49] awk 带条件
来源：http://kil.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kvp.yj202588.top

[R50] awk 求和
来源：http://ohz.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://hew.hcnkem.com

[R51] 排序去重取前几
来源：http://zxq.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gnw.zdqjudy.top

[R52] 统计行数
来源：http://ohy.xuanzx.com

wc -l a.txt
来源：http://lwq.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://yzv.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lla.jyoumei.cn

[R54] 比较两个文件
来源：http://aeh.hysaishi.cn

diff a.txt b.txt
来源：http://kjk.hnqzz.top

[R55] 压缩与解压
来源：http://ssf.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rpx.cucudq.cn

[R56] 远程拷贝
来源：http://lnn.yangfankeji.com

scp file user@host:/path/
来源：http://kfs.cdnleiting.top

[R57] 远程执行命令
来源：http://ekd.quarkkingdee.top

ssh user@host 'uptime'
来源：http://ymd.gaohongyu789.top

[R58] 下载文件
来源：http://cms.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxv.jinqigfzy.top

[R59] 发 POST JSON
来源：http://anu.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cgg.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://pfb.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aip.tarul.cn

[R61] 磁盘占用
来源：http://cgi.jqgufenzy.top

df -h;  du -sh *
来源：http://jat.yj202588.top

[R62] 找最占空间的文件
来源：http://twv.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://tak.zycfv.cn

[R63] 内存与进程
来源：http://zbh.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://nxj.zhoulong.xyz

[R64] 结束进程
来源：http://pcm.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://adb.zhijiandao.cn

[R65] 查看端口占用
来源：http://zcy.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://odw.zhongyouzk.top

[R66] 定时任务
来源：http://zbv.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://ghn.wangdashe.top

[R67] 生成随机十六进制串
来源：http://jrl.jqgufenzy.top

openssl rand -hex 16
来源：http://msa.0kj1m.cn

[R68] 计算文件校验值
来源：http://xyb.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://qxu.ydjk.org.cn

[R69] 生成随机密码
来源：http://bsk.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://fil.hammf.cn

[R70] 时间戳与互转
来源：http://nrk.hesvh.cn

date +%s;  date -d @1700000000
来源：http://dez.mhx1999.top

[R71] 日期格式化
来源：http://ovz.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sdf.sweek.top

[R72] 等待端口就绪
来源：http://vsk.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jef.jqgufenzy.top

[R73] 分割大日志
来源：http://arg.jinqigfzy.top

split -l 1000 big.log part_
来源：http://set.xylfe.cn

[R74] 批量重命名
来源：http://qet.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jct.sxryk.cn

[R75] 导出环境变量
来源：http://atv.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://nzk.gogol.net.cn

[R76] 使用临时文件
来源：http://uhd.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yhh.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://plv.haohaochexian.top

read -rp "请输入: " ans
来源：http://iiz.zdbjq.cn

[R78] 交互式菜单
来源：http://oau.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ifz.yj202588.top

[R79] 解析命令行选项
来源：http://qvo.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsn.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://sgt.chenjidiqi.icu

time ./run.sh
来源：http://xip.fengsongda.top

================================================================================
来源：http://unl.sxryk.cn

S. C / C++ 专题
来源：http://bgy.jianghu66.top

================================================================================
来源：http://mjd.gaohongyu789.top

[S01] C：Hello World
来源：http://vdm.bjfxy.top

#include <stdio.h>
来源：http://ykq.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lyi.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://oiv.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://kci.sweek.top

[S03] C：读入整数
来源：http://qou.yonumen.top

int x; scanf("%d", &x);
来源：http://run.sysykeji.top

[S04] C：字符串复制
来源：http://gaw.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ruz.ivvv.top

[S05] C：字符串长度
来源：http://xeo.pycfn.com

strlen(s)
来源：http://xxl.xinyue.icu

[S06] C：字符串比较
来源：http://otd.yueranfly.top

strcmp(a, b) == 0
来源：http://eem.zhengqikj.top

[S07] C：数组遍历求和
来源：http://ylm.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wdo.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://egl.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exl.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://goh.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lzu.zhengqikj.top

[S10] C：指针与解引用
来源：http://ihn.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://wzr.hnqzz.top

[S11] C：逐行读文件
来源：http://sts.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://clj.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tkd.gzhubu.top

fclose(f);
来源：http://qug.jinyuanbaomall.cn

[S12] C：写文件
来源：http://osu.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://opj.zdbjq.cn

[S13] C：宏定义
来源：http://xfx.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tna.0kj1m.cn

[S14] C：枚举
来源：http://cmo.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://ghr.nanxinkj.top

[S15] C：类型转换
来源：http://nqq.jlsjyb.cn

(double) a / b
来源：http://cbh.jyoumei.cn

[S16] C：位操作置位
来源：http://kmx.zhoulong.xyz

x |= (1 << 3);
来源：http://dtk.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://zhg.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://six.tian-w.cn

[S18] C：命令行参数
来源：http://bea.52xcode.cn

int main(int argc, char **argv)
来源：http://ukn.c1oappe.top

[S19] C：快速排序
来源：http://tdq.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uov.zhoulong.xyz

[S20] C：二分查找
来源：http://xfj.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yzi.jianghu66.top

[S21] C：字符类别判断
来源：http://nrs.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnr.mhx1999.top

[S22] C：字符串转数字
来源：http://cjj.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://qlm.havefunace.top

[S23] C：随机数
来源：http://kpd.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rji.gzhubu.top

[S24] C：获取本地时间
来源：http://vwu.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gnd.gotoacloud.top

[S25] C：内存拷贝
来源：http://jrc.iojbl.cn

memcpy(dst, src, n);
来源：http://avk.hongshengwenyu.top

[S26] C：内存清零
来源：http://zqd.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://xwq.zhoulong.xyz

[S27] C：定义常量
来源：http://pgu.jiagoushi.top

const double PI = 3.14159;
来源：http://sux.shzxlz.cn

[S28] C：静态变量
来源：http://uwk.gotoacloud.top

static int counter = 0;
来源：http://mpk.yfazqb.com

[S29] C：变参函数
来源：http://bqn.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kvt.shangyingyoupin.top

[S30] C：头文件保护
来源：http://ltt.shangyingyoupin.top

#ifndef X_H
来源：http://lpq.zhongyouzk.top

#define X_H
来源：http://zmi.iojbl.cn

#endif
来源：http://yyy.52xcode.cn

[S31] C++：Hello World
来源：http://zxc.dashuyun.cn


<!-- 参考信息 -->