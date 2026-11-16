代发 wailian999

ANALYZE TABLE users;
来源：http://wbu.52xcode.cn

[Q71] 查看建表语句
来源：http://yia.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wig.wangdashe.top

[Q72] 查看索引
来源：http://wej.c1oappe.top

SHOW INDEX FROM users;
来源：http://ktn.tanke756.top

[Q73] 查看表状态
来源：http://kum.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tsj.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://tmn.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eys.fzhhl.top

[Q75] 日期格式化
来源：http://dnp.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cfs.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pme.mhx1999.top

[Q76] 按天统计
来源：http://rvt.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ioe.gaohongyu789.top

[Q77] 时间加减
来源：http://hye.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ujb.pycfn.com

[Q78] 当前时间
来源：http://xza.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dsb.nanxuanxn.top

[Q79] 字符串拼接
来源：http://txu.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lqa.jlsjyb.cn

[Q80] 字符串截取
来源：http://zkv.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gsw.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://pvx.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zuz.cashguo.top

[Q82] 字符长度与字节长度
来源：http://abd.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rhv.xinyue.icu

[Q83] 大小写转换
来源：http://kyf.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://arn.chenzaomai.com

[Q84] 去除首尾空格
来源：http://bsn.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://xdw.jqgufenzy.top

[Q85] 数值取整
来源：http://rhb.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bqy.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://imo.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wwo.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://hyr.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wpn.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://ced.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jwq.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sis.ydzc1.top

[Q89] 判断表是否存在
来源：http://gjr.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pqy.uphjek.com

[Q90] 生成序号列
来源：http://yen.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uqc.0kj1m.cn

================================================================================
来源：http://vxh.hongshengwenyu.top

R. Bash 专题
来源：http://erj.jianghu66.top

================================================================================
来源：http://byx.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://ajp.gzhubu.top

#!/usr/bin/env bash
来源：http://zps.svipenyu.cn

set -euo pipefail
来源：http://wyf.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://fqz.haohaochexian.top

name="Tom"; echo "$name"
来源：http://xzi.jqgufenzy.top

[R03] 只读变量
来源：http://tzr.redwolf501.top

readonly PI=3.14
来源：http://vyv.yfazqb.com

[R04] 位置参数
来源：http://qzc.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zdu.daxiang520.top

[R05] 参数默认值
来源：http://lkp.zhaomingkeji.xyz

name="${1:-default}"
来源：http://tca.dashuyun.cn

[R06] 判断命令是否存在
来源：http://wzp.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cop.yongpay.top

[R07] if 判断文件
来源：http://lah.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xie.ydjk.org.cn

[R08] 数值比较
来源：http://rji.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zqn.shuidangran.top

[R09] 字符串比较
来源：http://mjq.shangyingyoupin.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mjl.zhiwuduotai.top

[R10] 正则匹配
来源：http://ybh.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qbk.gaohongyu789.top

[R11] case 多分支
来源：http://jcf.yanxiufei.cn

case "$1" in
来源：http://kip.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://ubw.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://vwd.yonumen.top

*)     echo "未知命令" ;;
来源：http://hfz.wangshuangyany.cn

esac
来源：http://klm.jianghu66.top

[R12] for 遍历文件
来源：http://cff.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://iwb.0kj1m.cn

[R13] for 计数循环
来源：http://raa.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://ziq.yj202588.top

[R14] C 风格 for
来源：http://ymb.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dxj.yuanzhike.top

[R15] while 逐行读文件
来源：http://sch.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dkl.sjlbkw.cn

[R16] until 等待条件
来源：http://lad.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zrs.epnwcf.com

[R17] 数组定义与取值
来源：http://sny.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ppy.fehbvm.com

[R18] 遍历数组
来源：http://jgx.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdp.ppjwa.cn

[R19] 数组长度
来源：http://rzl.sufxvd.cn

echo "${#arr[@]}"
来源：http://ltt.hcnkem.com

[R20] 关联数组（字典）
来源：http://xby.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://udu.sufxvd.cn

[R21] 字符串长度
来源：http://rvm.tian-w.cn

echo "${#s}"
来源：http://kby.jinqigufen.top

[R22] 截取子串
来源：http://upl.hywenlv.cn

echo "${s:0:5}"
来源：http://gda.feifeiyinyue.top

[R23] 字符串替换
来源：http://scs.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pgs.birdmap.top

[R24] 大小写转换
来源：http://wfq.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://ilp.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://enu.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://knu.yfazqb.com

[R26] 命令替换
来源：http://elv.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://ljl.ywan-chungtsiang.top

[R27] 算术展开
来源：http://ebi.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://kew.haohaochexian.top

[R28] 浮点运算
来源：http://mab.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://pfk.xinyue.icu

[R29] 定义函数
来源：http://msf.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qha.hysaishi.cn

[R30] 函数返回状态码
来源：http://rpx.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://oaf.fehbvm.com

[R31] 局部变量
来源：http://agt.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://xws.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://yko.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://otx.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://ovb.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dtd.ybcxt.top

[R34] 退出时清理
来源：http://fog.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://sie.zdqjudy.top

[R35] 后台执行并等待
来源：http://cbt.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bmm.fengsongda.top

[R36] 并发执行多个任务
来源：http://gox.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bvw.andypj.xyz

[R37] 把输出赋给变量
来源：http://oci.tian-w.cn

files=$(ls -1)
来源：http://jjk.jinqigfzy.top

[R38] 管道串联
来源：http://jvh.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://gng.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://uyw.fktsv.cn

cmd > out.log 2>&1
来源：http://nmo.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://hkt.zhijiandao.cn

echo "log" >> out.log
来源：http://tyq.zdqjudy.top

[R41] 丢弃输出
来源：http://rtr.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://ubb.tian-w.cn

[R42] 输入重定向
来源：http://lxy.dianchejie.cn

wc -l < a.txt
来源：http://pfw.xuanzx.com

[R43] 按名字查找文件
来源：http://kfc.sweek.top

find . -name "*.log" -type f
来源：http://cnz.sjlbkw.cn

[R44] 按修改时间查找
来源：http://coc.zycfv.cn

find . -mtime -7 -type f
来源：http://gbw.hnqzz.top

[R45] 批量删除
来源：http://sni.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://rxq.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://joo.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kvc.ppjwa.cn

[R47] sed 单行替换
来源：http://jpk.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yxg.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://ern.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://gjl.vehdjk.com

[R49] awk 带条件
来源：http://kzs.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gae.shangyingyoupin.top

[R50] awk 求和
来源：http://jgy.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://cno.sxryk.cn

[R51] 排序去重取前几
来源：http://tts.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jgu.fzhhl.top

[R52] 统计行数
来源：http://dhw.tanke756.top

wc -l a.txt
来源：http://jda.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://lcd.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vqu.zdbjq.cn

[R54] 比较两个文件
来源：http://gkf.birdmap.top

diff a.txt b.txt
来源：http://uce.yonumen.top

[R55] 压缩与解压
来源：http://ozt.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kvp.yuxming.cn

[R56] 远程拷贝
来源：http://ltx.zdqjudy.top

scp file user@host:/path/
来源：http://hkt.hongshengwenyu.top

[R57] 远程执行命令
来源：http://mop.yuanzhike.top

ssh user@host 'uptime'
来源：http://hcx.epnwcf.com

[R58] 下载文件
来源：http://ceb.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://arf.sweek.top

[R59] 发 POST JSON
来源：http://zqe.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vli.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://sll.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uos.fengsongda.top

[R61] 磁盘占用
来源：http://yeu.daxiang520.top

df -h;  du -sh *
来源：http://ppq.cdnleiting.top

[R62] 找最占空间的文件
来源：http://fys.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://obm.bbcook.cn

[R63] 内存与进程
来源：http://uug.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://cvo.chenzaomai.com

[R64] 结束进程
来源：http://wjl.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ksf.fehbvm.com

[R65] 查看端口占用
来源：http://yqa.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nyq.bbcook.cn

[R66] 定时任务
来源：http://edk.chenlongwang.top

crontab -e;  crontab -l
来源：http://zpr.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://vil.hfpthk.cn

openssl rand -hex 16
来源：http://vat.jlsjyb.cn

[R68] 计算文件校验值
来源：http://axq.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://nxd.wangshuangyany.cn

[R69] 生成随机密码
来源：http://lla.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://ejb.tanke756.top

[R70] 时间戳与互转
来源：http://cke.fehbvm.com

date +%s;  date -d @1700000000
来源：http://lrc.zhijiandao.cn

[R71] 日期格式化
来源：http://fco.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ozf.fehbvm.com

[R72] 等待端口就绪
来源：http://ypk.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nvh.gogol.net.cn

[R73] 分割大日志
来源：http://qzi.yj20258888.top

split -l 1000 big.log part_
来源：http://vae.fehbvm.com

[R74] 批量重命名
来源：http://qfg.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mwj.pycfn.com

[R75] 导出环境变量
来源：http://uub.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tvg.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://rhd.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://guo.tanke756.top

[R77] 读取用户输入
来源：http://sfg.nwbrower.top

read -rp "请输入: " ans
来源：http://tdm.hnqzz.top

[R78] 交互式菜单
来源：http://eap.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cer.jlsjyb.cn

[R79] 解析命令行选项
来源：http://jle.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wme.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://swk.hnqzz.top

time ./run.sh
来源：http://kyl.aibaodan.cn

================================================================================
来源：http://rrt.hongshengwenyu.top

S. C / C++ 专题
来源：http://alx.hywenlv.cn

================================================================================
来源：http://lur.nanxinkj.top

[S01] C：Hello World
来源：http://vnx.sufxvd.cn

#include <stdio.h>
来源：http://jki.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fth.meibo888.top

[S02] C：变量与格式化输出
来源：http://jyc.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://qok.sxryk.cn

[S03] C：读入整数
来源：http://aju.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://xds.wangdashe.top

[S04] C：字符串复制
来源：http://kpt.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ncg.sjlbkw.cn

[S05] C：字符串长度
来源：http://ifh.fehbvm.com

strlen(s)
来源：http://lrg.nanxuanxn.top

[S06] C：字符串比较
来源：http://gbo.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://cjl.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://czz.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ajc.yj20258.top

[S08] C：动态内存分配与释放
来源：http://man.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xhy.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://jzb.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jpw.hnqzz.top

[S10] C：指针与解引用
来源：http://roa.uphjek.com

int *p = &a;  *p = 5;
来源：http://ttq.cheryme.top

[S11] C：逐行读文件
来源：http://kan.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://beu.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qae.tarul.cn

fclose(f);
来源：http://ssp.yj20258888.top

[S12] C：写文件
来源：http://gin.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://evs.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://ghx.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kpz.sweek.top

[S14] C：枚举
来源：http://ibn.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://moo.gaohongyu789.top

[S15] C：类型转换
来源：http://uga.c1oappe.top

(double) a / b
来源：http://qzr.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://uot.jinqigufen.top

x |= (1 << 3);
来源：http://frv.yvedp.cn

[S17] C：安全拼接字符串
来源：http://ohr.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dep.yanxiufei.cn

[S18] C：命令行参数
来源：http://erg.meibo888.top

int main(int argc, char **argv)
来源：http://eir.aizwys.cn

[S19] C：快速排序
来源：http://edv.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nsg.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://cnx.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tjs.sufxvd.cn

[S21] C：字符类别判断
来源：http://mql.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfx.yj202588.top

[S22] C：字符串转数字
来源：http://fco.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://xru.zhaomingkeji.xyz

[S23] C：随机数
来源：http://ohm.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://boh.nwbrower.top

[S24] C：获取本地时间
来源：http://njr.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://csh.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://bit.zhongyouzk.top

memcpy(dst, src, n);
来源：http://zyv.sufxvd.cn

[S26] C：内存清零
来源：http://fcn.sysykeji.top

memset(a, 0, sizeof a);
来源：http://abo.gotoacloud.top

[S27] C：定义常量
来源：http://shj.pycfn.com

const double PI = 3.14159;
来源：http://yzt.gotoacloud.top

[S28] C：静态变量
来源：http://cfi.zhixingplan.top

static int counter = 0;
来源：http://bph.redwolf501.top

[S29] C：变参函数
来源：http://ckt.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mrx.xinyue.icu

[S30] C：头文件保护
来源：http://fhx.zhongyouzk.top

#ifndef X_H
来源：http://sxt.cashguo.top

#define X_H
来源：http://hjs.vehdjk.com

#endif
来源：http://nkx.havefunace.top

[S31] C++：Hello World
来源：http://eez.jinqigfzy.top

#include <iostream>
来源：http://swr.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://ghd.guannengcc.top

[S32] C++：字符串
来源：http://aee.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://ewu.xylfe.cn

[S33] C++：vector 增删
来源：http://ksi.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://obu.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://aqr.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://geo.yj202588.top

[S35] C++：map
来源：http://qlz.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://puu.sjlbkw.cn

[S36] C++：unordered_map
来源：http://hoo.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zwv.guannengcc.top

[S37] C++：set
来源：http://erv.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bll.mhx1999.top

[S38] C++：排序
来源：http://jom.yongpay.top

std::sort(v.begin(), v.end());
来源：http://cyx.yonumen.top

[S39] C++：自定义比较器排序
来源：http://arj.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://idz.hongshengwenyu.top

[S40] C++：查找元素
来源：http://jaq.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmc.wangshuangyany.cn


<!-- 参考信息 -->