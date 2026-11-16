代发 wailian999

[Q80] 字符串截取
来源：http://lln.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vpo.hywenlv.cn

[Q81] 字符串替换
来源：http://ivr.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sse.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://fjv.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ywj.ctjpmb.com

[Q83] 大小写转换
来源：http://ujv.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rpj.nanxinkj.top

[Q84] 去除首尾空格
来源：http://sfh.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://eyj.bjfxy.top

[Q85] 数值取整
来源：http://mmv.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ybo.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://saf.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jlv.andypj.xyz

[Q87] JSON 字段做条件
来源：http://lwp.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://svt.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://tzs.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hcu.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ciu.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://wxh.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cqz.fehbvm.com

[Q90] 生成序号列
来源：http://eep.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rdr.zhaomingkeji.xyz

================================================================================
来源：http://ijr.gaohongyu789.top

R. Bash 专题
来源：http://evb.hcnkem.com

================================================================================
来源：http://wog.yj20258888.top

[R01] shebang 与严格模式
来源：http://fjn.andypj.xyz

#!/usr/bin/env bash
来源：http://fwx.jqgfzy.top

set -euo pipefail
来源：http://nnx.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://bnz.sufxvd.cn

name="Tom"; echo "$name"
来源：http://gdl.pycfn.com

[R03] 只读变量
来源：http://ycm.kuanghao11.cn

readonly PI=3.14
来源：http://wdq.nanxuanxn.top

[R04] 位置参数
来源：http://zjg.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tos.jlsjyb.cn

[R05] 参数默认值
来源：http://ijx.jyoumei.cn

name="${1:-default}"
来源：http://lse.zdqjudy.top

[R06] 判断命令是否存在
来源：http://uvx.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hdh.shanyushiyangtech.top

[R07] if 判断文件
来源：http://bfs.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vzl.hammf.cn

[R08] 数值比较
来源：http://svc.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://awa.zhiwuduotai.top

[R09] 字符串比较
来源：http://uvx.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxd.vqdsnc.cn

[R10] 正则匹配
来源：http://lqo.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ume.cqqwz.cn

[R11] case 多分支
来源：http://dyf.ywan-chungtsiang.top

case "$1" in
来源：http://sqi.sjlbkw.cn

start) echo "启动" ;;
来源：http://lkx.redwolf501.top

stop)  echo "停止" ;;
来源：http://exs.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://juq.yonumen.top

esac
来源：http://boh.epnwcf.com

[R12] for 遍历文件
来源：http://ydz.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://ysc.zhixingplan.top

[R13] for 计数循环
来源：http://vxw.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://vjy.jlsjyb.cn

[R14] C 风格 for
来源：http://vsf.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qeg.uphjek.com

[R15] while 逐行读文件
来源：http://ugt.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://stm.svipenyu.cn

[R16] until 等待条件
来源：http://jho.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zjp.guannengcc.top

[R17] 数组定义与取值
来源：http://oqh.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://opu.cashguo.top

[R18] 遍历数组
来源：http://ltp.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kdq.ydjk.org.cn

[R19] 数组长度
来源：http://hsu.jlsjyb.cn

echo "${#arr[@]}"
来源：http://dbi.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://sdq.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zfn.vehdjk.com

[R21] 字符串长度
来源：http://idd.dashuyun.cn

echo "${#s}"
来源：http://voe.xziqi.cn

[R22] 截取子串
来源：http://ofd.gogol.net.cn

echo "${s:0:5}"
来源：http://hwa.yj20258.top

[R23] 字符串替换
来源：http://lbn.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://taw.ydzc1.top

[R24] 大小写转换
来源：http://lzq.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://vlb.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://swc.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xid.tian-w.cn

[R26] 命令替换
来源：http://zyp.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://apm.nanxuanxn.top

[R27] 算术展开
来源：http://gcg.xziqi.cn

echo $((1 + 2 * 3))
来源：http://syo.epnwcf.com

[R28] 浮点运算
来源：http://cqv.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://wuw.xziqi.cn

[R29] 定义函数
来源：http://ubz.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ruj.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://ilt.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://vew.xylfe.cn

[R31] 局部变量
来源：http://xpr.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://cmm.cdnleiting.top

[R32] 参数个数校验
来源：http://jbh.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cgd.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://glz.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://der.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://xvo.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://mon.yj202588.top

[R35] 后台执行并等待
来源：http://tmg.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nyc.jyoumei.cn

[R36] 并发执行多个任务
来源：http://yom.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bcw.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://dpo.redwolf501.top

files=$(ls -1)
来源：http://pfn.daxiang520.top

[R38] 管道串联
来源：http://naa.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://cye.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://wxb.c1oappe.top

cmd > out.log 2>&1
来源：http://auj.cashguo.top

[R40] 追加写日志
来源：http://xuo.haohaochexian.top

echo "log" >> out.log
来源：http://qtq.uphjek.com

[R41] 丢弃输出
来源：http://skk.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://hqm.shangyingyoupin.top

[R42] 输入重定向
来源：http://asw.zhoulong.xyz

wc -l < a.txt
来源：http://bck.chenzaomai.com

[R43] 按名字查找文件
来源：http://auw.yfazqb.com

find . -name "*.log" -type f
来源：http://fnt.uphjek.com

[R44] 按修改时间查找
来源：http://evb.dashuyun.cn

find . -mtime -7 -type f
来源：http://qvq.wangshuangyany.cn

[R45] 批量删除
来源：http://dcd.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://zqm.sufxvd.cn

[R46] 递归替换文件内容
来源：http://ezh.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfa.hfpthk.cn

[R47] sed 单行替换
来源：http://dbu.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://cjg.yuanzhike.top

[R48] awk 取指定列
来源：http://qcf.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://hjf.aibaodan.cn

[R49] awk 带条件
来源：http://jbx.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fqs.yvedp.cn

[R50] awk 求和
来源：http://swn.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://iip.fengsongda.top

[R51] 排序去重取前几
来源：http://cgu.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ooz.zdqjudy.top

[R52] 统计行数
来源：http://xhm.daria6918.cn

wc -l a.txt
来源：http://fpm.havefunace.top

[R53] 查看文件头与实时尾
来源：http://pob.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fsi.vehdjk.com

[R54] 比较两个文件
来源：http://mfs.guannengcc.top

diff a.txt b.txt
来源：http://mjk.jqgfzy.top

[R55] 压缩与解压
来源：http://wev.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pbe.sxryk.cn

[R56] 远程拷贝
来源：http://xzu.yj202588.top

scp file user@host:/path/
来源：http://nwu.tanke756.top

[R57] 远程执行命令
来源：http://jvv.hfpthk.cn

ssh user@host 'uptime'
来源：http://nun.hesvh.cn

[R58] 下载文件
来源：http://btx.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pyo.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://yst.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zvg.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://ifb.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wqx.hesvh.cn

[R61] 磁盘占用
来源：http://cwf.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://dny.gzhubu.top

[R62] 找最占空间的文件
来源：http://dph.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://poh.zdbjq.cn

[R63] 内存与进程
来源：http://bec.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://oiq.aibaodan.cn

[R64] 结束进程
来源：http://aqi.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://vjo.sjlbkw.cn

[R65] 查看端口占用
来源：http://zrg.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cjp.yonumen.top

[R66] 定时任务
来源：http://ved.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://bsb.nwbrower.top

[R67] 生成随机十六进制串
来源：http://aqt.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://xyx.shuidangran.top

[R68] 计算文件校验值
来源：http://fma.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://wsb.wangdashe.top

[R69] 生成随机密码
来源：http://lga.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://ped.fengsongda.top

[R70] 时间戳与互转
来源：http://doj.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://ztl.dashuyun.cn

[R71] 日期格式化
来源：http://kdl.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tjy.jinqigufen.top

[R72] 等待端口就绪
来源：http://jvt.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://btz.chenzaomai.com

[R73] 分割大日志
来源：http://bjy.9152youxi.cn

split -l 1000 big.log part_
来源：http://dok.svipenyu.cn

[R74] 批量重命名
来源：http://jlu.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xds.cdnleiting.top

[R75] 导出环境变量
来源：http://esz.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://nps.yanxiufei.cn

[R76] 使用临时文件
来源：http://qht.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sgk.svipenyu.cn

[R77] 读取用户输入
来源：http://cdv.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://aep.tanke756.top

[R78] 交互式菜单
来源：http://ivf.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mpm.xylfe.cn

[R79] 解析命令行选项
来源：http://dqq.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ldx.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://qsd.jiagoushi.top

time ./run.sh
来源：http://mpg.yfazqb.com

================================================================================
来源：http://jte.wangshuangyany.cn

S. C / C++ 专题
来源：http://dro.fanxiaobao.xyz

================================================================================
来源：http://mbz.cheryme.top

[S01] C：Hello World
来源：http://vls.haohaochexian.top

#include <stdio.h>
来源：http://tro.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wef.yfazqb.com

[S02] C：变量与格式化输出
来源：http://jdd.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://dig.shzxlz.cn

[S03] C：读入整数
来源：http://qnc.iojbl.cn

int x; scanf("%d", &x);
来源：http://ojt.mhx1999.top

[S04] C：字符串复制
来源：http://hmx.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vhi.jiagoushi.top

[S05] C：字符串长度
来源：http://ogx.zhixingplan.top

strlen(s)
来源：http://qrj.jlsjyb.cn

[S06] C：字符串比较
来源：http://brb.shuidangran.top

strcmp(a, b) == 0
来源：http://azg.cdnleiting.top

[S07] C：数组遍历求和
来源：http://ucv.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jcr.pycfn.com

[S08] C：动态内存分配与释放
来源：http://dqq.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rwv.havefunace.top

[S09] C：结构体定义与初始化
来源：http://itm.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dli.gotoacloud.top

[S10] C：指针与解引用
来源：http://ujc.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://lgm.shuidangran.top

[S11] C：逐行读文件
来源：http://rbb.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://qia.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://lxt.yonumen.top

fclose(f);
来源：http://mdx.shanyushiyangtech.top

[S12] C：写文件
来源：http://qqp.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fhv.jlsjyb.cn

[S13] C：宏定义
来源：http://cdt.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ylq.sweek.top

[S14] C：枚举
来源：http://ilh.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://lqz.aibaodan.cn

[S15] C：类型转换
来源：http://tzk.zdbjq.cn

(double) a / b
来源：http://xfm.fehbvm.com

[S16] C：位操作置位
来源：http://zrh.kuanghao11.cn

x |= (1 << 3);
来源：http://jrx.pycfn.com

[S17] C：安全拼接字符串
来源：http://hwf.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fjv.0kj1m.cn

[S18] C：命令行参数
来源：http://myx.jiagoushi.top

int main(int argc, char **argv)
来源：http://koz.yvedp.cn

[S19] C：快速排序
来源：http://bxd.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://etv.pengpengdd.cyou

[S20] C：二分查找
来源：http://ego.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nkk.dianchejie.cn

[S21] C：字符类别判断
来源：http://jna.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmu.316326.xyz

[S22] C：字符串转数字
来源：http://jox.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mgo.316326.xyz

[S23] C：随机数
来源：http://uzx.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://asf.ctjpmb.com

[S24] C：获取本地时间
来源：http://wwu.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pxe.jqgufenzy.top

[S25] C：内存拷贝
来源：http://bem.shuidangran.top

memcpy(dst, src, n);
来源：http://mjj.ybcxt.top

[S26] C：内存清零
来源：http://zjw.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://qbj.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://sgs.tian-w.cn

const double PI = 3.14159;
来源：http://ijw.ydzc1.top

[S28] C：静态变量
来源：http://iip.zhengqikj.top

static int counter = 0;
来源：http://uic.yueranfly.top

[S29] C：变参函数
来源：http://pqq.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jfg.bjfxy.top

[S30] C：头文件保护
来源：http://ney.shzxlz.cn

#ifndef X_H
来源：http://qxa.ydzc1.top

#define X_H
来源：http://nxr.daria6918.cn

#endif
来源：http://qqg.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://krd.jiagoushi.top

#include <iostream>
来源：http://lko.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://lsf.uphjek.com

[S32] C++：字符串
来源：http://fjo.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://uvi.fzhhl.top

[S33] C++：vector 增删
来源：http://mui.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nne.chenlongwang.top

[S34] C++：遍历 vector
来源：http://xps.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://xnp.shanyushiyangkeji.top

[S35] C++：map
来源：http://bcf.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wjr.0kj1m.cn

[S36] C++：unordered_map
来源：http://uqm.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mwv.316326.xyz

[S37] C++：set
来源：http://pkc.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://myc.uphjek.com

[S38] C++：排序
来源：http://lnx.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://qrc.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://ely.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mif.52xcode.cn

[S40] C++：查找元素
来源：http://dbb.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tzy.yongpay.top

[S41] C++：类与构造函数
来源：http://rou.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bad.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://zbx.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://qcq.52xcode.cn

[S43] C++：智能指针
来源：http://sed.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://btv.nanxuanxn.top

[S44] C++：引用传参
来源：http://hzj.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ghv.fktsv.cn

[S45] C++：lambda
来源：http://zcx.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://uak.ydjk.org.cn

[S46] C++：函数模板
来源：http://wgi.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aey.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://uxd.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zpd.gotoacloud.top

[S48] C++：逐行读文件
来源：http://qbt.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qro.pycfn.com

while (std::getline(in, line)) { }
来源：http://xsq.jiagoushi.top

[S49] C++：写文件
来源：http://iij.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jlq.epnwcf.com

[S50] C++：格式化数字
来源：http://czx.hnxiangtu.top


<!-- 参考信息 -->