代发 wailian999

[Q82] 字符长度与字节长度
来源：http://tzg.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mey.yangfankeji.com

[Q83] 大小写转换
来源：http://qaf.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://snl.tianlin.xyz

[Q84] 去除首尾空格
来源：http://ykn.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://qyt.hongshengwenyu.top

[Q85] 数值取整
来源：http://awp.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rnx.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://qqm.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pfo.gzhubu.top

[Q87] JSON 字段做条件
来源：http://nzq.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wfp.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://irr.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://any.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://boa.ydzc1.top

[Q89] 判断表是否存在
来源：http://wcx.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://inv.0kj1m.cn

[Q90] 生成序号列
来源：http://mxa.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jpz.chenjidiqi.icu

================================================================================
来源：http://pso.xuetiantiany.cn

R. Bash 专题
来源：http://rru.birdmap.top

================================================================================
来源：http://cif.yuanzhike.top

[R01] shebang 与严格模式
来源：http://qaa.nwbrower.top

#!/usr/bin/env bash
来源：http://oyi.gaohongyu789.top

set -euo pipefail
来源：http://fpz.ppjwa.cn

[R02] 变量赋值与使用
来源：http://vru.yfazqb.com

name="Tom"; echo "$name"
来源：http://zwz.jyoumei.cn

[R03] 只读变量
来源：http://rzo.jinyuanbaomall.cn

readonly PI=3.14
来源：http://wgq.yfazqb.com

[R04] 位置参数
来源：http://fqf.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://drq.gogol.net.cn

[R05] 参数默认值
来源：http://meb.guannengcc.top

name="${1:-default}"
来源：http://wxl.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://fyi.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ldh.pycfn.com

[R07] if 判断文件
来源：http://dyj.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qkx.chenlongwang.top

[R08] 数值比较
来源：http://vmk.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vwv.chenjidiqi.icu

[R09] 字符串比较
来源：http://cbz.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mya.hnxiangtu.top

[R10] 正则匹配
来源：http://gpo.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cfl.jlsjyb.cn

[R11] case 多分支
来源：http://ypb.yuxming.cn

case "$1" in
来源：http://kip.iojbl.cn

start) echo "启动" ;;
来源：http://bwy.sweek.top

stop)  echo "停止" ;;
来源：http://umy.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://fcf.nanxuanxn.top

esac
来源：http://wjz.iojbl.cn

[R12] for 遍历文件
来源：http://och.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://pkj.chenjidiqi.icu

[R13] for 计数循环
来源：http://oir.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://dlq.jinqigufen.top

[R14] C 风格 for
来源：http://shr.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vxz.aibaodan.cn

[R15] while 逐行读文件
来源：http://clt.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nfv.yj20258888.top

[R16] until 等待条件
来源：http://exs.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sws.zdqjudy.top

[R17] 数组定义与取值
来源：http://mlc.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://enn.zhoulong.xyz

[R18] 遍历数组
来源：http://goi.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uqn.zhaomingkeji.xyz

[R19] 数组长度
来源：http://prm.andypj.xyz

echo "${#arr[@]}"
来源：http://pqh.shuidangran.top

[R20] 关联数组（字典）
来源：http://rpp.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hnc.hywenlv.cn

[R21] 字符串长度
来源：http://ktd.redwolf501.top

echo "${#s}"
来源：http://zrl.52xcode.cn

[R22] 截取子串
来源：http://okz.ydjk.org.cn

echo "${s:0:5}"
来源：http://yto.havefunace.top

[R23] 字符串替换
来源：http://zer.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://puv.cheryme.top

[R24] 大小写转换
来源：http://czx.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://bcf.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://yjv.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gdn.zhiwuduotai.top

[R26] 命令替换
来源：http://kpg.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://qce.hongshengwenyu.top

[R27] 算术展开
来源：http://hvw.daria6918.cn

echo $((1 + 2 * 3))
来源：http://gvc.yuanzhike.top

[R28] 浮点运算
来源：http://yne.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://lxx.uphjek.com

[R29] 定义函数
来源：http://faw.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zrt.52xcode.cn

[R30] 函数返回状态码
来源：http://psq.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://kwf.ybcxt.top

[R31] 局部变量
来源：http://poj.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://ruv.andypj.xyz

[R32] 参数个数校验
来源：http://fhf.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ajb.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://gyb.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://atc.birdmap.top

[R34] 退出时清理
来源：http://szi.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://ncm.zhoulong.xyz

[R35] 后台执行并等待
来源：http://fyq.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xan.sweek.top

[R36] 并发执行多个任务
来源：http://sbl.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yjm.tarul.cn

[R37] 把输出赋给变量
来源：http://xgw.yongpay.top

files=$(ls -1)
来源：http://znt.pengpengdd.cyou

[R38] 管道串联
来源：http://oqv.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://hkw.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://uvu.xylfe.cn

cmd > out.log 2>&1
来源：http://pjh.gaohongyu789.top

[R40] 追加写日志
来源：http://ysw.jlsjyb.cn

echo "log" >> out.log
来源：http://ypk.zhengqikj.top

[R41] 丢弃输出
来源：http://pha.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://qfk.316326.xyz

[R42] 输入重定向
来源：http://izd.zhongyouzk.top

wc -l < a.txt
来源：http://rjo.epnwcf.com

[R43] 按名字查找文件
来源：http://qam.fehbvm.com

find . -name "*.log" -type f
来源：http://zpd.sxryk.cn

[R44] 按修改时间查找
来源：http://lta.ctjpmb.com

find . -mtime -7 -type f
来源：http://vkr.hcnkem.com

[R45] 批量删除
来源：http://kqk.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://nsc.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://drz.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uir.wangdashe.top

[R47] sed 单行替换
来源：http://stc.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://aiy.hongshengwenyu.top

[R48] awk 取指定列
来源：http://gzw.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://ofc.yuanzhike.top

[R49] awk 带条件
来源：http://nia.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://osb.shanyushiyangtech.top

[R50] awk 求和
来源：http://gjo.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dkg.gzhubu.top

[R51] 排序去重取前几
来源：http://bip.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wrj.pycfn.com

[R52] 统计行数
来源：http://jls.dianchejie.cn

wc -l a.txt
来源：http://uct.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://dkl.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wwd.sxryk.cn

[R54] 比较两个文件
来源：http://mbo.shangyingyoupin.top

diff a.txt b.txt
来源：http://rtn.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://ssu.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://azl.xziqi.cn

[R56] 远程拷贝
来源：http://jag.jlsjyb.cn

scp file user@host:/path/
来源：http://jjg.yj20258888.top

[R57] 远程执行命令
来源：http://elt.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://ftb.chenzaomai.com

[R58] 下载文件
来源：http://zlq.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hgj.yj20258888.top

[R59] 发 POST JSON
来源：http://efs.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lei.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://hmg.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wei.52xcode.cn

[R61] 磁盘占用
来源：http://ckd.uphjek.com

df -h;  du -sh *
来源：http://btf.zdbjq.cn

[R62] 找最占空间的文件
来源：http://nhm.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://zzz.ivvv.top

[R63] 内存与进程
来源：http://wus.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://lca.andypj.xyz

[R64] 结束进程
来源：http://kfw.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://qzu.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://rvo.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://icl.zdbjq.cn

[R66] 定时任务
来源：http://mzv.gotoacloud.top

crontab -e;  crontab -l
来源：http://ppf.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://wpr.hfpthk.cn

openssl rand -hex 16
来源：http://zbz.zhixingplan.top

[R68] 计算文件校验值
来源：http://jdq.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://vih.jqgufenzy.top

[R69] 生成随机密码
来源：http://gqe.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://eag.hywenlv.cn

[R70] 时间戳与互转
来源：http://irw.yj20258.top

date +%s;  date -d @1700000000
来源：http://ttc.vehdjk.com

[R71] 日期格式化
来源：http://ftq.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://efx.ydzc1.top

[R72] 等待端口就绪
来源：http://dxr.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kpd.zycfv.cn

[R73] 分割大日志
来源：http://nbd.yvedp.cn

split -l 1000 big.log part_
来源：http://mkh.yongpay.top

[R74] 批量重命名
来源：http://yer.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mtj.hfpthk.cn

[R75] 导出环境变量
来源：http://bxy.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://eij.tarul.cn

[R76] 使用临时文件
来源：http://kby.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nkm.yangfankeji.com

[R77] 读取用户输入
来源：http://yrk.zhixingplan.top

read -rp "请输入: " ans
来源：http://kuv.havefunace.top

[R78] 交互式菜单
来源：http://wws.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bjh.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://kxr.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://axd.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://eym.gotoacloud.top

time ./run.sh
来源：http://cld.fengsongda.top

================================================================================
来源：http://qrr.vqdsnc.cn

S. C / C++ 专题
来源：http://xct.havefunace.top

================================================================================
来源：http://lae.hammf.cn

[S01] C：Hello World
来源：http://hux.fengsongda.top

#include <stdio.h>
来源：http://zuk.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kvs.hcnkem.com

[S02] C：变量与格式化输出
来源：http://oog.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://iqm.mhx1999.top

[S03] C：读入整数
来源：http://efc.yangfankeji.com

int x; scanf("%d", &x);
来源：http://dkx.bbcook.cn

[S04] C：字符串复制
来源：http://ivf.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://mbu.xylfe.cn

[S05] C：字符串长度
来源：http://ryu.chenlongwang.top

strlen(s)
来源：http://emi.gotoacloud.top

[S06] C：字符串比较
来源：http://ptd.yonumen.top

strcmp(a, b) == 0
来源：http://dfd.tarul.cn

[S07] C：数组遍历求和
来源：http://uvm.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bmr.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://ydi.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dfn.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://ygf.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://abv.sufxvd.cn

[S10] C：指针与解引用
来源：http://rce.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://okn.nanxinkj.top

[S11] C：逐行读文件
来源：http://vba.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pyk.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wxf.svipenyu.cn

fclose(f);
来源：http://gvr.nanxuanxn.top

[S12] C：写文件
来源：http://suv.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://afs.52xcode.cn

[S13] C：宏定义
来源：http://umu.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nmh.jqgfzy.top

[S14] C：枚举
来源：http://pkb.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://dtu.xuetiantiany.cn

[S15] C：类型转换
来源：http://rol.ybcxt.top

(double) a / b
来源：http://cxl.yj202588.top

[S16] C：位操作置位
来源：http://okr.sjlbkw.cn

x |= (1 << 3);
来源：http://bsl.xylfe.cn

[S17] C：安全拼接字符串
来源：http://ems.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jba.hfpthk.cn

[S18] C：命令行参数
来源：http://qrn.meibo888.top

int main(int argc, char **argv)
来源：http://eht.meibo888.top

[S19] C：快速排序
来源：http://jks.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qju.fehbvm.com

[S20] C：二分查找
来源：http://kdg.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wvi.tianlin.xyz

[S21] C：字符类别判断
来源：http://cnx.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tad.epnwcf.com

[S22] C：字符串转数字
来源：http://rzh.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://qsa.jinqigufen.top

[S23] C：随机数
来源：http://ixy.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lfp.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://uzf.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uip.iojbl.cn

[S25] C：内存拷贝
来源：http://dlf.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://wvr.sweek.top

[S26] C：内存清零
来源：http://gth.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://tdi.daxiang520.top

[S27] C：定义常量
来源：http://ejj.pycfn.com

const double PI = 3.14159;
来源：http://wfw.ydjk.org.cn

[S28] C：静态变量
来源：http://wte.kuanghao11.cn

static int counter = 0;
来源：http://kzh.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://twf.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rty.cashguo.top

[S30] C：头文件保护
来源：http://jou.guowangkeji.top

#ifndef X_H
来源：http://zxu.nwbrower.top

#define X_H
来源：http://wyr.zhiwuduotai.top

#endif
来源：http://rsx.hesvh.cn

[S31] C++：Hello World
来源：http://wjm.gotoacloud.top

#include <iostream>
来源：http://xwo.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://dzc.vehdjk.com

[S32] C++：字符串
来源：http://vpj.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://nwi.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://aku.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hti.birdmap.top

[S34] C++：遍历 vector
来源：http://xsz.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://wuj.fktsv.cn

[S35] C++：map
来源：http://try.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ndf.yongpay.top

[S36] C++：unordered_map
来源：http://mwv.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iof.52xcode.cn

[S37] C++：set
来源：http://kdi.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gob.hnqzz.top

[S38] C++：排序
来源：http://pwj.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://rpa.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://kkf.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hgf.hysaishi.cn

[S40] C++：查找元素
来源：http://feg.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zyz.shuidangran.top

[S41] C++：类与构造函数
来源：http://xkm.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vak.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://rmw.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://rok.jiagoushi.top

[S43] C++：智能指针
来源：http://vhp.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://rft.jqgfzy.top

[S44] C++：引用传参
来源：http://arp.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://wsa.vqdsnc.cn

[S45] C++：lambda
来源：http://bir.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://qyv.zhiwuduotai.top

[S46] C++：函数模板
来源：http://ccb.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://roy.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://eny.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://euc.hnqzz.top

[S48] C++：逐行读文件
来源：http://qsm.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://pnc.pycfn.com

while (std::getline(in, line)) { }
来源：http://gkk.fanxiaobao.xyz

[S49] C++：写文件
来源：http://yyu.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fwn.zhoulong.xyz

[S50] C++：格式化数字
来源：http://oqc.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txj.yongpay.top

[S51] C++：显式类型转换
来源：http://tgt.fehbvm.com

static_cast<double>(a) / b
来源：http://yfg.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://yyt.ybcxt.top


<!-- 参考信息 -->