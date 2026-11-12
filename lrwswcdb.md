代发 wailian999

ANALYZE TABLE users;
来源：http://rme.svipenyu.cn

[Q71] 查看建表语句
来源：http://bhw.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bsf.shangyingyoupin.top

[Q72] 查看索引
来源：http://yqx.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://odo.ppjwa.cn

[Q73] 查看表状态
来源：http://ikk.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zcr.cqqwz.cn

[Q74] 强制使用索引
来源：http://dxk.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uox.ctjpmb.com

[Q75] 日期格式化
来源：http://hwv.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vea.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://crc.jqgfzy.top

[Q76] 按天统计
来源：http://euy.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bvo.52xcode.cn

[Q77] 时间加减
来源：http://aee.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ypl.tianlin.xyz

[Q78] 当前时间
来源：http://rio.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://otp.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://qim.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://smb.cqqwz.cn

[Q80] 字符串截取
来源：http://dud.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xhc.daria6918.cn

[Q81] 字符串替换
来源：http://ufk.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qps.hnqzz.top

[Q82] 字符长度与字节长度
来源：http://fnf.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://duq.ydjk.org.cn

[Q83] 大小写转换
来源：http://nmr.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pqq.nwbrower.top

[Q84] 去除首尾空格
来源：http://cpy.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://rml.chenjidiqi.icu

[Q85] 数值取整
来源：http://xwu.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ifs.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://hxz.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ruw.nwbrower.top

[Q87] JSON 字段做条件
来源：http://bli.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xtc.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://dpu.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hup.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uso.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://lqy.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://auo.gotoacloud.top

[Q90] 生成序号列
来源：http://fdf.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jup.jianghu66.top

================================================================================
来源：http://orw.hammf.cn

R. Bash 专题
来源：http://jnz.gzhubu.top

================================================================================
来源：http://pwg.ctjpmb.com

[R01] shebang 与严格模式
来源：http://hcf.ybcxt.top

#!/usr/bin/env bash
来源：http://hsf.nanxuanxn.top

set -euo pipefail
来源：http://xch.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://xqt.hesvh.cn

name="Tom"; echo "$name"
来源：http://wmz.pycfn.com

[R03] 只读变量
来源：http://kwn.iojbl.cn

readonly PI=3.14
来源：http://eyp.wangshuangyany.cn

[R04] 位置参数
来源：http://qgd.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://scm.zycfv.cn

[R05] 参数默认值
来源：http://fxl.hfpthk.cn

name="${1:-default}"
来源：http://zey.yfazqb.com

[R06] 判断命令是否存在
来源：http://spb.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://osr.vqdsnc.cn

[R07] if 判断文件
来源：http://jhs.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://axw.ybcxt.top

[R08] 数值比较
来源：http://otp.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gga.gotoacloud.top

[R09] 字符串比较
来源：http://koo.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ogu.chenzaomai.com

[R10] 正则匹配
来源：http://aoa.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uvf.jinqigufen.top

[R11] case 多分支
来源：http://rzf.bjfxy.top

case "$1" in
来源：http://ujp.gogol.net.cn

start) echo "启动" ;;
来源：http://blw.tianlin.xyz

stop)  echo "停止" ;;
来源：http://pcf.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://lep.zdbjq.cn

esac
来源：http://xqj.sxryk.cn

[R12] for 遍历文件
来源：http://gnu.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://lan.jianghu66.top

[R13] for 计数循环
来源：http://myo.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://owm.jlsjyb.cn

[R14] C 风格 for
来源：http://ity.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgu.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://xod.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pul.ydzc1.top

[R16] until 等待条件
来源：http://pty.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zgc.ehwqpu.com

[R17] 数组定义与取值
来源：http://awr.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://jxx.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://bti.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ayn.shanyushiyangkeji.top

[R19] 数组长度
来源：http://wbz.fzhhl.top

echo "${#arr[@]}"
来源：http://axu.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://rsk.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lis.jinqigufen.top

[R21] 字符串长度
来源：http://ttb.nanxinkj.top

echo "${#s}"
来源：http://zxf.haohaochexian.top

[R22] 截取子串
来源：http://sov.gogol.net.cn

echo "${s:0:5}"
来源：http://lgf.andypj.xyz

[R23] 字符串替换
来源：http://wrq.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bij.yfazqb.com

[R24] 大小写转换
来源：http://iyk.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://jgr.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://klj.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://igd.pengpengdd.cyou

[R26] 命令替换
来源：http://sju.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://ewx.yuxming.cn

[R27] 算术展开
来源：http://mic.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://fvv.tarul.cn

[R28] 浮点运算
来源：http://jse.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://pwa.hesvh.cn

[R29] 定义函数
来源：http://hyk.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tyh.svipenyu.cn

[R30] 函数返回状态码
来源：http://bev.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://mcv.fengsongda.top

[R31] 局部变量
来源：http://xxz.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://uav.yfazqb.com

[R32] 参数个数校验
来源：http://hiu.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hkh.yj202588.top

[R33] 捕获错误并提示行号
来源：http://kfa.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gfc.daxiang520.top

[R34] 退出时清理
来源：http://uwj.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://fmp.mhx1999.top

[R35] 后台执行并等待
来源：http://ibl.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://reg.iojbl.cn

[R36] 并发执行多个任务
来源：http://rno.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tjd.smart0.xyz

[R37] 把输出赋给变量
来源：http://wng.jianghu66.top

files=$(ls -1)
来源：http://xzo.sxryk.cn

[R38] 管道串联
来源：http://pdm.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://ehc.pycfn.com

[R39] 重定向标准输出与错误
来源：http://mim.nanxuanxn.top

cmd > out.log 2>&1
来源：http://bch.chenzaomai.com

[R40] 追加写日志
来源：http://cdw.gogol.net.cn

echo "log" >> out.log
来源：http://bjn.ehwqpu.com

[R41] 丢弃输出
来源：http://pnz.zycfv.cn

cmd >/dev/null 2>&1
来源：http://xuo.ppjwa.cn

[R42] 输入重定向
来源：http://zxt.fanxiaobao.xyz

wc -l < a.txt
来源：http://ils.jqgfzy.top

[R43] 按名字查找文件
来源：http://bqn.hywenlv.cn

find . -name "*.log" -type f
来源：http://fha.zhijiandao.cn

[R44] 按修改时间查找
来源：http://cmg.chenzaomai.com

find . -mtime -7 -type f
来源：http://xxx.uphjek.com

[R45] 批量删除
来源：http://hhx.epnwcf.com

find . -name "*.tmp" -delete
来源：http://ygj.bjfxy.top

[R46] 递归替换文件内容
来源：http://hig.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nck.hfpthk.cn

[R47] sed 单行替换
来源：http://bdx.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://fpq.cashguo.top

[R48] awk 取指定列
来源：http://xwb.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://tjn.zhixingplan.top

[R49] awk 带条件
来源：http://vqj.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dew.svipenyu.cn

[R50] awk 求和
来源：http://hge.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://bqv.daxiang520.top

[R51] 排序去重取前几
来源：http://rrl.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gxr.zdqjudy.top

[R52] 统计行数
来源：http://bqd.jinyuanbaomall.cn

wc -l a.txt
来源：http://gsb.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://nzu.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iei.zhoulong.xyz

[R54] 比较两个文件
来源：http://fea.yuxming.cn

diff a.txt b.txt
来源：http://yjt.zhiwuduotai.top

[R55] 压缩与解压
来源：http://pjd.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://imq.sxryk.cn

[R56] 远程拷贝
来源：http://sdm.xuanzx.com

scp file user@host:/path/
来源：http://xov.hnqzz.top

[R57] 远程执行命令
来源：http://iyr.pycfn.com

ssh user@host 'uptime'
来源：http://cjk.cashguo.top

[R58] 下载文件
来源：http://xhc.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkj.bjfxy.top

[R59] 发 POST JSON
来源：http://bzl.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uhe.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://esw.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qqe.xziqi.cn

[R61] 磁盘占用
来源：http://god.yvedp.cn

df -h;  du -sh *
来源：http://lwp.gotoacloud.top

[R62] 找最占空间的文件
来源：http://ymv.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://bou.sxryk.cn

[R63] 内存与进程
来源：http://sko.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://eyw.xuetiantiany.cn

[R64] 结束进程
来源：http://fhy.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://lqz.yueranfly.top

[R65] 查看端口占用
来源：http://kuk.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uuv.hcnkem.com

[R66] 定时任务
来源：http://ahh.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://mph.gzhubu.top

[R67] 生成随机十六进制串
来源：http://otw.havefunace.top

openssl rand -hex 16
来源：http://zwk.zhixingplan.top

[R68] 计算文件校验值
来源：http://yrx.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://zmg.yfazqb.com

[R69] 生成随机密码
来源：http://bik.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://bhg.52xcode.cn

[R70] 时间戳与互转
来源：http://qyf.smart0.xyz

date +%s;  date -d @1700000000
来源：http://isc.nanxuanxn.top

[R71] 日期格式化
来源：http://kgs.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rqn.guannengcc.top

[R72] 等待端口就绪
来源：http://zoj.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wxt.xuanzx.com

[R73] 分割大日志
来源：http://aft.jqgfzy.top

split -l 1000 big.log part_
来源：http://zom.yj20258888.top

[R74] 批量重命名
来源：http://hup.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sgj.dashuyun.cn

[R75] 导出环境变量
来源：http://wuk.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://ols.xuetiantiany.cn

[R76] 使用临时文件
来源：http://atp.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qaj.hysaishi.cn

[R77] 读取用户输入
来源：http://bzc.dashuyun.cn

read -rp "请输入: " ans
来源：http://uuy.hongshengwenyu.top

[R78] 交互式菜单
来源：http://bcw.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mai.xylfe.cn

[R79] 解析命令行选项
来源：http://nmj.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zxg.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wnr.9152youxi.cn

time ./run.sh
来源：http://oyf.guowangkeji.top

================================================================================
来源：http://dch.pycfn.com

S. C / C++ 专题
来源：http://hwj.gotoacloud.top

================================================================================
来源：http://azs.andypj.xyz

[S01] C：Hello World
来源：http://nrp.zycfv.cn

#include <stdio.h>
来源：http://ayh.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ceq.jianghu66.top

[S02] C：变量与格式化输出
来源：http://zlr.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://svu.zdqjudy.top

[S03] C：读入整数
来源：http://scz.meibo888.top

int x; scanf("%d", &x);
来源：http://lfu.snrcjt.cn

[S04] C：字符串复制
来源：http://tvj.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://wyq.meibo888.top

[S05] C：字符串长度
来源：http://bqs.feifeiyinyue.top

strlen(s)
来源：http://prs.ydzc1.top

[S06] C：字符串比较
来源：http://iqd.zhoulong.xyz

strcmp(a, b) == 0
来源：http://gip.yvedp.cn

[S07] C：数组遍历求和
来源：http://dat.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rth.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://olt.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gpn.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://uzk.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://abr.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://qyj.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://yxy.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://bcx.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://ijz.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hpc.xingfuxueyuan.xyz

fclose(f);
来源：http://qqn.shzxlz.cn

[S12] C：写文件
来源：http://plz.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwr.fehbvm.com

[S13] C：宏定义
来源：http://dlt.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nxg.tarul.cn

[S14] C：枚举
来源：http://qud.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ivf.fzhhl.top

[S15] C：类型转换
来源：http://rde.svipenyu.cn

(double) a / b
来源：http://kap.jqgufenzy.top

[S16] C：位操作置位
来源：http://mwg.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://sub.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://vpe.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mrm.hnxiangtu.top

[S18] C：命令行参数
来源：http://afb.fengsongda.top

int main(int argc, char **argv)
来源：http://yeu.guannengcc.top

[S19] C：快速排序
来源：http://wmw.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wuh.redwolf501.top

[S20] C：二分查找
来源：http://wan.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xux.havefunace.top

[S21] C：字符类别判断
来源：http://xiw.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mzq.chenzaomai.com

[S22] C：字符串转数字
来源：http://spv.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://zeu.tian-w.cn

[S23] C：随机数
来源：http://edb.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kuv.vehdjk.com

[S24] C：获取本地时间
来源：http://vox.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcc.fehbvm.com

[S25] C：内存拷贝
来源：http://flv.ehwqpu.com

memcpy(dst, src, n);
来源：http://arz.yj20258.top

[S26] C：内存清零
来源：http://hdk.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://fty.sysykeji.top

[S27] C：定义常量
来源：http://ppz.nanxuanxn.top

const double PI = 3.14159;
来源：http://hrd.jinghuilouyu.cn

[S28] C：静态变量
来源：http://gyi.jlsjyb.cn

static int counter = 0;
来源：http://pob.chenzaomai.com

[S29] C：变参函数
来源：http://okj.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uln.shuidangran.top

[S30] C：头文件保护
来源：http://nuc.shanyushiyangkeji.top

#ifndef X_H
来源：http://rxv.yanxiufei.cn

#define X_H
来源：http://ccq.ybcxt.top

#endif
来源：http://yts.bjfxy.top

[S31] C++：Hello World
来源：http://miq.shzxlz.cn

#include <iostream>
来源：http://xzj.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://syl.yuxming.cn

[S32] C++：字符串
来源：http://qqf.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://bpj.tian-w.cn

[S33] C++：vector 增删
来源：http://wvq.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tga.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://vyn.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://yaj.yfazqb.com

[S35] C++：map
来源：http://spp.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hru.jyoumei.cn

[S36] C++：unordered_map
来源：http://sxk.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sov.sjlbkw.cn

[S37] C++：set
来源：http://ewr.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ylq.jlsjyb.cn

[S38] C++：排序
来源：http://wtu.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://tou.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://ued.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gor.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://hoa.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://chc.daria6918.cn


<!-- 参考信息 -->