代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://huu.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://hqs.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yzr.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gdu.shangyingyoupin.top

[Q76] 按天统计
来源：http://rfr.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xpv.c1oappe.top

[Q77] 时间加减
来源：http://pyq.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://div.xylfe.cn

[Q78] 当前时间
来源：http://zvj.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://grm.mhx1999.top

[Q79] 字符串拼接
来源：http://xss.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qpo.52xcode.cn

[Q80] 字符串截取
来源：http://fom.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cvd.ybcxt.top

[Q81] 字符串替换
来源：http://yne.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tme.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://vue.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dsh.jlsjyb.cn

[Q83] 大小写转换
来源：http://htu.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ibw.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://ozo.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://gla.zdqjudy.top

[Q85] 数值取整
来源：http://vdl.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kti.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://xme.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cjd.sxryk.cn

[Q87] JSON 字段做条件
来源：http://ejt.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrg.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://mop.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hyn.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://any.gotoacloud.top

[Q89] 判断表是否存在
来源：http://cbx.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcb.yvedp.cn

[Q90] 生成序号列
来源：http://ydg.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://myc.yvedp.cn

================================================================================
来源：http://tko.gaohongyu789.top

R. Bash 专题
来源：http://xgd.fktsv.cn

================================================================================
来源：http://ngf.wangdashe.top

[R01] shebang 与严格模式
来源：http://ugx.0kj1m.cn

#!/usr/bin/env bash
来源：http://mhj.redwolf501.top

set -euo pipefail
来源：http://foy.iojbl.cn

[R02] 变量赋值与使用
来源：http://jor.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://uri.guannengcc.top

[R03] 只读变量
来源：http://hqc.ydzc1.top

readonly PI=3.14
来源：http://fuo.fengsongda.top

[R04] 位置参数
来源：http://poo.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iue.sweek.top

[R05] 参数默认值
来源：http://hrp.ivvv.top

name="${1:-default}"
来源：http://wwj.wangdashe.top

[R06] 判断命令是否存在
来源：http://asr.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zpc.yj20258888.top

[R07] if 判断文件
来源：http://ciq.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nyv.smart0.xyz

[R08] 数值比较
来源：http://ayb.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mwj.andypj.xyz

[R09] 字符串比较
来源：http://lku.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udf.zhoulong.xyz

[R10] 正则匹配
来源：http://bqg.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fdu.zhiwuduotai.top

[R11] case 多分支
来源：http://vpy.hysaishi.cn

case "$1" in
来源：http://zae.tian-w.cn

start) echo "启动" ;;
来源：http://qfa.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://vph.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://inc.ydzc1.top

esac
来源：http://pjh.ydzc1.top

[R12] for 遍历文件
来源：http://itd.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://fss.shzxlz.cn

[R13] for 计数循环
来源：http://rgi.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://gjy.zhengqikj.top

[R14] C 风格 for
来源：http://ayz.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ilq.ydzc1.top

[R15] while 逐行读文件
来源：http://ujh.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://brk.fengsongda.top

[R16] until 等待条件
来源：http://sym.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wez.0kj1m.cn

[R17] 数组定义与取值
来源：http://eup.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hrx.xuetiantiany.cn

[R18] 遍历数组
来源：http://gxb.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ixa.xinyue.icu

[R19] 数组长度
来源：http://kih.jiagoushi.top

echo "${#arr[@]}"
来源：http://hxg.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://oox.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://myk.epnwcf.com

[R21] 字符串长度
来源：http://adh.aibaodan.cn

echo "${#s}"
来源：http://csg.ehwqpu.com

[R22] 截取子串
来源：http://jxc.svipenyu.cn

echo "${s:0:5}"
来源：http://wkn.hnqzz.top

[R23] 字符串替换
来源：http://dbx.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://njv.ydzc1.top

[R24] 大小写转换
来源：http://erp.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xjp.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://oan.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xzq.sysykeji.top

[R26] 命令替换
来源：http://mud.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://zbi.yueranfly.top

[R27] 算术展开
来源：http://vri.daria6918.cn

echo $((1 + 2 * 3))
来源：http://jqn.tian-w.cn

[R28] 浮点运算
来源：http://jtl.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://ewh.jlsjyb.cn

[R29] 定义函数
来源：http://vzv.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cna.bjfxy.top

[R30] 函数返回状态码
来源：http://lxg.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://szd.zhixingplan.top

[R31] 局部变量
来源：http://dal.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://alb.shangyingyoupin.top

[R32] 参数个数校验
来源：http://frh.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mqk.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://ynk.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tos.jinghuilouyu.cn

[R34] 退出时清理
来源：http://hjq.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://wiz.epnwcf.com

[R35] 后台执行并等待
来源：http://yde.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://xbh.meibo888.top

[R36] 并发执行多个任务
来源：http://uau.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfd.sysykeji.top

[R37] 把输出赋给变量
来源：http://rdz.pycfn.com

files=$(ls -1)
来源：http://wck.hongshengwenyu.top

[R38] 管道串联
来源：http://eys.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://amy.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://jdu.mhx1999.top

cmd > out.log 2>&1
来源：http://bpg.yj20258.top

[R40] 追加写日志
来源：http://jft.gzhubu.top

echo "log" >> out.log
来源：http://lbc.gaohongyu789.top

[R41] 丢弃输出
来源：http://pmf.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://jhh.sxryk.cn

[R42] 输入重定向
来源：http://oms.hysaishi.cn

wc -l < a.txt
来源：http://foh.hnxiangtu.top

[R43] 按名字查找文件
来源：http://xsl.jqgufenzy.top

find . -name "*.log" -type f
来源：http://wtl.ctjpmb.com

[R44] 按修改时间查找
来源：http://gks.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://ico.chenlongwang.top

[R45] 批量删除
来源：http://lww.hesvh.cn

find . -name "*.tmp" -delete
来源：http://kkr.nwbrower.top

[R46] 递归替换文件内容
来源：http://nlr.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zcv.fzhhl.top

[R47] sed 单行替换
来源：http://seo.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://kes.c1oappe.top

[R48] awk 取指定列
来源：http://ybb.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://alc.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://owi.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uob.haohaochexian.top

[R50] awk 求和
来源：http://dfc.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpr.zhijiandao.cn

[R51] 排序去重取前几
来源：http://wma.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://vfm.c1oappe.top

[R52] 统计行数
来源：http://baa.gzhubu.top

wc -l a.txt
来源：http://bvx.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://kqk.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ufk.hesvh.cn

[R54] 比较两个文件
来源：http://mqx.fktsv.cn

diff a.txt b.txt
来源：http://hlx.zdbjq.cn

[R55] 压缩与解压
来源：http://pfn.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ads.kuanghao11.cn

[R56] 远程拷贝
来源：http://vmr.fktsv.cn

scp file user@host:/path/
来源：http://gwy.fehbvm.com

[R57] 远程执行命令
来源：http://edm.cdnleiting.top

ssh user@host 'uptime'
来源：http://fhl.hysaishi.cn

[R58] 下载文件
来源：http://frb.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zsu.fzhhl.top

[R59] 发 POST JSON
来源：http://jvn.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rqv.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://xsy.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mni.xinyue.icu

[R61] 磁盘占用
来源：http://him.sufxvd.cn

df -h;  du -sh *
来源：http://mne.52xcode.cn

[R62] 找最占空间的文件
来源：http://zvv.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://kai.chenlongwang.top

[R63] 内存与进程
来源：http://ktx.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://vlg.shzxlz.cn

[R64] 结束进程
来源：http://oep.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://ysq.yj20258.top

[R65] 查看端口占用
来源：http://bpi.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mxx.smart0.xyz

[R66] 定时任务
来源：http://xjj.sxryk.cn

crontab -e;  crontab -l
来源：http://ijl.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://fkm.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://def.ydjk.org.cn

[R68] 计算文件校验值
来源：http://jav.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mpy.xuetiantiany.cn

[R69] 生成随机密码
来源：http://wqv.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://ozt.andypj.xyz

[R70] 时间戳与互转
来源：http://lka.mhx1999.top

date +%s;  date -d @1700000000
来源：http://ckc.nanxuanxn.top

[R71] 日期格式化
来源：http://hvb.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rlv.ehwqpu.com

[R72] 等待端口就绪
来源：http://kkk.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hek.aibaodan.cn

[R73] 分割大日志
来源：http://rty.gogol.net.cn

split -l 1000 big.log part_
来源：http://vrg.52xcode.cn

[R74] 批量重命名
来源：http://vhn.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://axj.yuanzhike.top

[R75] 导出环境变量
来源：http://hue.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://hrw.havefunace.top

[R76] 使用临时文件
来源：http://enl.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fsp.nanxuanxn.top

[R77] 读取用户输入
来源：http://rgc.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://vmg.yj202588.top

[R78] 交互式菜单
来源：http://dnl.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://umd.sjlbkw.cn

[R79] 解析命令行选项
来源：http://hqq.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zwl.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://hot.birdmap.top

time ./run.sh
来源：http://nfs.sweek.top

================================================================================
来源：http://hkm.nwbrower.top

S. C / C++ 专题
来源：http://uks.guowangkeji.top

================================================================================
来源：http://wzr.bjfxy.top

[S01] C：Hello World
来源：http://lhx.ctjpmb.com

#include <stdio.h>
来源：http://kjp.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hlj.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://zjq.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://ogp.guannengcc.top

[S03] C：读入整数
来源：http://ccy.vehdjk.com

int x; scanf("%d", &x);
来源：http://ivh.aibaodan.cn

[S04] C：字符串复制
来源：http://acw.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://fgh.cucudq.cn

[S05] C：字符串长度
来源：http://hgj.c1oappe.top

strlen(s)
来源：http://vxa.xuanzx.com

[S06] C：字符串比较
来源：http://etc.jinqigufen.top

strcmp(a, b) == 0
来源：http://kqc.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://gzj.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://obw.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://kic.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcj.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://dmh.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rxm.fehbvm.com

[S10] C：指针与解引用
来源：http://ajn.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://ljt.c1oappe.top

[S11] C：逐行读文件
来源：http://fge.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://jov.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rir.uphjek.com

fclose(f);
来源：http://lre.dashuyun.cn

[S12] C：写文件
来源：http://jki.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vvv.daria6918.cn

[S13] C：宏定义
来源：http://obt.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agu.zycfv.cn

[S14] C：枚举
来源：http://ivz.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://mcs.epnwcf.com

[S15] C：类型转换
来源：http://nxx.sufxvd.cn

(double) a / b
来源：http://gyt.svipenyu.cn

[S16] C：位操作置位
来源：http://ipr.xziqi.cn

x |= (1 << 3);
来源：http://cfa.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://eoc.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sdy.vqdsnc.cn

[S18] C：命令行参数
来源：http://nqo.zhoulong.xyz

int main(int argc, char **argv)
来源：http://yxh.jlsjyb.cn

[S19] C：快速排序
来源：http://dnn.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://axd.hesvh.cn

[S20] C：二分查找
来源：http://qfh.uphjek.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ukz.svipenyu.cn

[S21] C：字符类别判断
来源：http://fzl.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yuf.nwbrower.top

[S22] C：字符串转数字
来源：http://irq.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://bev.bjfxy.top

[S23] C：随机数
来源：http://dla.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dyh.aibaodan.cn

[S24] C：获取本地时间
来源：http://gnb.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rla.tian-w.cn

[S25] C：内存拷贝
来源：http://cvd.gzhubu.top

memcpy(dst, src, n);
来源：http://qki.smart0.xyz

[S26] C：内存清零
来源：http://set.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://eny.cheryme.top

[S27] C：定义常量
来源：http://vje.yj202588.top

const double PI = 3.14159;
来源：http://lft.haohaochexian.top

[S28] C：静态变量
来源：http://yvl.sweek.top

static int counter = 0;
来源：http://xfq.tarul.cn

[S29] C：变参函数
来源：http://kid.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://stp.zhijiandao.cn

[S30] C：头文件保护
来源：http://rcv.meibo888.top

#ifndef X_H
来源：http://tva.dianchejie.cn

#define X_H
来源：http://vdk.hfpthk.cn

#endif
来源：http://qwb.hammf.cn

[S31] C++：Hello World
来源：http://ubu.gaohongyu789.top

#include <iostream>
来源：http://gkp.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://rqi.cheryme.top

[S32] C++：字符串
来源：http://qkv.yongpay.top

std::string s = "hi";  s += "!";
来源：http://ufc.yonumen.top

[S33] C++：vector 增删
来源：http://vol.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://alb.zdbjq.cn

[S34] C++：遍历 vector
来源：http://ctv.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://fhg.vehdjk.com

[S35] C++：map
来源：http://chx.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://svv.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://apv.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dnq.xylfe.cn

[S37] C++：set
来源：http://tfw.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lpo.pycfn.com

[S38] C++：排序
来源：http://ghx.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://pkz.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://bhm.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://orq.cdnleiting.top

[S40] C++：查找元素
来源：http://dac.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://epg.316326.xyz

[S41] C++：类与构造函数
来源：http://fjy.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://geq.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://hnp.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://lib.tian-w.cn

[S43] C++：智能指针
来源：http://uyd.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://vvp.redwolf501.top

[S44] C++：引用传参
来源：http://wuw.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://fuu.xuanzx.com


<!-- 参考信息 -->