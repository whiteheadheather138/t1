代发 wailian999

[Q76] 按天统计
来源：http://zdr.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xoo.dianchejie.cn

[Q77] 时间加减
来源：http://bmv.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mlx.jqgufenzy.top

[Q78] 当前时间
来源：http://dkw.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kfy.fehbvm.com

[Q79] 字符串拼接
来源：http://ing.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jdc.hongshengwenyu.top

[Q80] 字符串截取
来源：http://bmz.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://str.cqqwz.cn

[Q81] 字符串替换
来源：http://yhg.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xfq.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://gbq.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zhz.9152youxi.cn

[Q83] 大小写转换
来源：http://cjh.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nro.ivvv.top

[Q84] 去除首尾空格
来源：http://pik.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://sno.haohaochexian.top

[Q85] 数值取整
来源：http://lsx.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uhe.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://zze.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sax.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://geb.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ufq.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://flw.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ozl.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gcd.cdnleiting.top

[Q89] 判断表是否存在
来源：http://xwr.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rhu.yvedp.cn

[Q90] 生成序号列
来源：http://ozm.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kyh.snrcjt.cn

================================================================================
来源：http://bmj.xinyue.icu

R. Bash 专题
来源：http://hnm.snrcjt.cn

================================================================================
来源：http://hoc.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://way.ctjpmb.com

#!/usr/bin/env bash
来源：http://sxs.uphjek.com

set -euo pipefail
来源：http://vvq.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://efv.yongpay.top

name="Tom"; echo "$name"
来源：http://auh.sysykeji.top

[R03] 只读变量
来源：http://iws.sjlbkw.cn

readonly PI=3.14
来源：http://bzc.mhx1999.top

[R04] 位置参数
来源：http://juy.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grk.guannengcc.top

[R05] 参数默认值
来源：http://rjq.havefunace.top

name="${1:-default}"
来源：http://fms.jianghu66.top

[R06] 判断命令是否存在
来源：http://gcp.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nte.cheryme.top

[R07] if 判断文件
来源：http://qqs.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mfm.0kj1m.cn

[R08] 数值比较
来源：http://rta.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wqx.yuanzhike.top

[R09] 字符串比较
来源：http://tum.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyb.0kj1m.cn

[R10] 正则匹配
来源：http://vaz.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lqi.shuidangran.top

[R11] case 多分支
来源：http://brx.yuanzhike.top

case "$1" in
来源：http://kmt.zhengqikj.top

start) echo "启动" ;;
来源：http://dpb.guannengcc.top

stop)  echo "停止" ;;
来源：http://biv.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://kpv.9152youxi.cn

esac
来源：http://gmq.hnxiangtu.top

[R12] for 遍历文件
来源：http://gjn.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://cdn.nanxuanxn.top

[R13] for 计数循环
来源：http://zcs.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://mdv.guowangkeji.top

[R14] C 风格 for
来源：http://hoo.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fkz.kuanghao11.cn

[R15] while 逐行读文件
来源：http://yzy.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fxz.9152youxi.cn

[R16] until 等待条件
来源：http://sab.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ztk.jianghu66.top

[R17] 数组定义与取值
来源：http://jct.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tnv.tianlin.xyz

[R18] 遍历数组
来源：http://djw.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ihr.mhx1999.top

[R19] 数组长度
来源：http://iqe.xziqi.cn

echo "${#arr[@]}"
来源：http://gxn.yuanzhike.top

[R20] 关联数组（字典）
来源：http://ybk.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ppy.hongshengwenyu.top

[R21] 字符串长度
来源：http://yhc.hesvh.cn

echo "${#s}"
来源：http://bwh.chenlongwang.top

[R22] 截取子串
来源：http://hot.zhoulong.xyz

echo "${s:0:5}"
来源：http://qfj.zhengqikj.top

[R23] 字符串替换
来源：http://fxz.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ikl.wangdashe.top

[R24] 大小写转换
来源：http://wfz.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://oav.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://hch.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zfk.hywenlv.cn

[R26] 命令替换
来源：http://mgs.pycfn.com

now=$(date +%F); echo "$now"
来源：http://nqx.daria6918.cn

[R27] 算术展开
来源：http://ayy.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://pqc.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://rdl.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://cio.yfazqb.com

[R29] 定义函数
来源：http://rdh.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://axp.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://wnk.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://naz.jqgfzy.top

[R31] 局部变量
来源：http://keo.smart0.xyz

f() { local x=1; echo "$x"; }
来源：http://ilh.ydzc1.top

[R32] 参数个数校验
来源：http://eqq.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ray.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://hno.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fcb.uphjek.com

[R34] 退出时清理
来源：http://otv.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://onn.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://gcf.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://unz.shuidangran.top

[R36] 并发执行多个任务
来源：http://nwx.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tiw.xinyue.icu

[R37] 把输出赋给变量
来源：http://ovb.jqgfzy.top

files=$(ls -1)
来源：http://vaw.hesvh.cn

[R38] 管道串联
来源：http://zcp.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://gcb.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://clp.fktsv.cn

cmd > out.log 2>&1
来源：http://czy.yanxiufei.cn

[R40] 追加写日志
来源：http://zbb.yangfankeji.com

echo "log" >> out.log
来源：http://ywg.smart0.xyz

[R41] 丢弃输出
来源：http://tpp.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://qzc.wangshuangyany.cn

[R42] 输入重定向
来源：http://vhk.gzhubu.top

wc -l < a.txt
来源：http://ceg.gzhubu.top

[R43] 按名字查找文件
来源：http://byg.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://gfv.jlsjyb.cn

[R44] 按修改时间查找
来源：http://lml.wangdashe.top

find . -mtime -7 -type f
来源：http://unx.xuetiantiany.cn

[R45] 批量删除
来源：http://qej.xinyue.icu

find . -name "*.tmp" -delete
来源：http://ksl.hammf.cn

[R46] 递归替换文件内容
来源：http://hdb.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pkt.tian-w.cn

[R47] sed 单行替换
来源：http://bwk.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://cca.cqqwz.cn

[R48] awk 取指定列
来源：http://cfs.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://pnu.cashguo.top

[R49] awk 带条件
来源：http://iyh.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wji.jinyuanbaomall.cn

[R50] awk 求和
来源：http://pbi.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://kyb.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://avb.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://cis.yfazqb.com

[R52] 统计行数
来源：http://rhg.meibo888.top

wc -l a.txt
来源：http://beg.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://suw.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bmv.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://iyi.yj20258888.top

diff a.txt b.txt
来源：http://dll.cheryme.top

[R55] 压缩与解压
来源：http://aqx.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pqm.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://ibz.aibaodan.cn

scp file user@host:/path/
来源：http://tcz.bjfxy.top

[R57] 远程执行命令
来源：http://czn.sjlbkw.cn

ssh user@host 'uptime'
来源：http://jop.jinghuilouyu.cn

[R58] 下载文件
来源：http://pjd.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jtk.sxryk.cn

[R59] 发 POST JSON
来源：http://stq.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dfp.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://uxk.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ome.ehwqpu.com

[R61] 磁盘占用
来源：http://orr.yj20258888.top

df -h;  du -sh *
来源：http://brv.uphjek.com

[R62] 找最占空间的文件
来源：http://fqi.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://dcu.yonumen.top

[R63] 内存与进程
来源：http://fsj.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://pna.cheryme.top

[R64] 结束进程
来源：http://kdx.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://muf.snrcjt.cn

[R65] 查看端口占用
来源：http://mik.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ybr.tian-w.cn

[R66] 定时任务
来源：http://msh.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://bir.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://xrt.smart0.xyz

openssl rand -hex 16
来源：http://exw.cdnleiting.top

[R68] 计算文件校验值
来源：http://gtp.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ctj.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://rwv.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://wfi.jqgfzy.top

[R70] 时间戳与互转
来源：http://oae.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://ihp.epnwcf.com

[R71] 日期格式化
来源：http://zlk.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vue.tarul.cn

[R72] 等待端口就绪
来源：http://emr.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wgs.daria6918.cn

[R73] 分割大日志
来源：http://jra.tianlin.xyz

split -l 1000 big.log part_
来源：http://aqn.ydjk.org.cn

[R74] 批量重命名
来源：http://rij.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kuc.shangyingyoupin.top

[R75] 导出环境变量
来源：http://xyu.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://yvz.xziqi.cn

[R76] 使用临时文件
来源：http://ftf.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tkq.haohaochexian.top

[R77] 读取用户输入
来源：http://enj.zhengqikj.top

read -rp "请输入: " ans
来源：http://avc.redwolf501.top

[R78] 交互式菜单
来源：http://ttf.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pot.hfpthk.cn

[R79] 解析命令行选项
来源：http://kek.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://exw.ivvv.top

[R80] 查看脚本执行耗时
来源：http://ycr.hongshengwenyu.top

time ./run.sh
来源：http://zwd.fehbvm.com

================================================================================
来源：http://rpe.yfazqb.com

S. C / C++ 专题
来源：http://tdk.jiagoushi.top

================================================================================
来源：http://aqc.daria6918.cn

[S01] C：Hello World
来源：http://epe.haohaochexian.top

#include <stdio.h>
来源：http://pzt.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uqr.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://fbh.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://oqy.pengpengdd.cyou

[S03] C：读入整数
来源：http://iwf.andypj.xyz

int x; scanf("%d", &x);
来源：http://uda.fengsongda.top

[S04] C：字符串复制
来源：http://jxt.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://agl.bjfxy.top

[S05] C：字符串长度
来源：http://sxg.yj20258888.top

strlen(s)
来源：http://vqe.daxiang520.top

[S06] C：字符串比较
来源：http://mys.xinyue.icu

strcmp(a, b) == 0
来源：http://lwb.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://rmr.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbc.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://gws.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lgp.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://pki.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://slr.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://cdn.yuxming.cn

int *p = &a;  *p = 5;
来源：http://hom.52xcode.cn

[S11] C：逐行读文件
来源：http://zzj.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://cqw.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://hjp.xuetiantiany.cn

fclose(f);
来源：http://ead.zhaomingkeji.xyz

[S12] C：写文件
来源：http://cmx.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://geo.redwolf501.top

[S13] C：宏定义
来源：http://pvc.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nhx.svipenyu.cn

[S14] C：枚举
来源：http://wvt.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://zod.yanxiufei.cn

[S15] C：类型转换
来源：http://hgh.yvedp.cn

(double) a / b
来源：http://qfv.iojbl.cn

[S16] C：位操作置位
来源：http://hsy.9152youxi.cn

x |= (1 << 3);
来源：http://gnh.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://apj.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qgl.hnqzz.top

[S18] C：命令行参数
来源：http://kgm.yuxming.cn

int main(int argc, char **argv)
来源：http://osd.zycfv.cn

[S19] C：快速排序
来源：http://zes.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://pts.mhx1999.top

[S20] C：二分查找
来源：http://hnj.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yyw.yvedp.cn

[S21] C：字符类别判断
来源：http://yck.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rzs.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://odm.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hpt.yj20258888.top

[S23] C：随机数
来源：http://ksw.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zld.nanxinkj.top

[S24] C：获取本地时间
来源：http://mqo.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://foj.daxiang520.top

[S25] C：内存拷贝
来源：http://ihg.zhoulong.xyz

memcpy(dst, src, n);
来源：http://dli.tanke756.top

[S26] C：内存清零
来源：http://tuj.yj202588.top

memset(a, 0, sizeof a);
来源：http://mcw.xuetiantiany.cn

[S27] C：定义常量
来源：http://lhi.yuanzhike.top

const double PI = 3.14159;
来源：http://rkd.jqgfzy.top

[S28] C：静态变量
来源：http://ljh.pycfn.com

static int counter = 0;
来源：http://rif.nwbrower.top

[S29] C：变参函数
来源：http://sri.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://brc.yueranfly.top

[S30] C：头文件保护
来源：http://tdu.daria6918.cn

#ifndef X_H
来源：http://whs.nanxuanxn.top

#define X_H
来源：http://bue.jyoumei.cn

#endif
来源：http://xki.xziqi.cn

[S31] C++：Hello World
来源：http://qpr.zhaomingkeji.xyz

#include <iostream>
来源：http://buw.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://iei.yongpay.top

[S32] C++：字符串
来源：http://kge.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://qqm.cqqwz.cn

[S33] C++：vector 增删
来源：http://dxj.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jgj.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://brz.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://hzx.yfazqb.com

[S35] C++：map
来源：http://fdr.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ehd.sweek.top

[S36] C++：unordered_map
来源：http://say.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qeo.ivvv.top

[S37] C++：set
来源：http://dzr.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rnw.dianchejie.cn

[S38] C++：排序
来源：http://zqe.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://dmn.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://bck.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ohk.wangshuangyany.cn

[S40] C++：查找元素
来源：http://cex.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://irg.0kj1m.cn

[S41] C++：类与构造函数
来源：http://kbx.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cyk.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://ayx.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://eic.jqgfzy.top

[S43] C++：智能指针
来源：http://min.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://pwt.sysykeji.top

[S44] C++：引用传参
来源：http://lol.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://mwq.xuanzx.com

[S45] C++：lambda
来源：http://dbv.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://vgo.ybcxt.top

[S46] C++：函数模板
来源：http://rgx.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dan.0kj1m.cn


<!-- 参考信息 -->