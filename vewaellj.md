代发 wailian999

[Q86] 读取 JSON 字段
来源：http://rjm.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bhq.yueranfly.top

[Q87] JSON 字段做条件
来源：http://uoa.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zdd.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://kjz.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://igj.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wik.9152youxi.cn

[Q89] 判断表是否存在
来源：http://xrj.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pxc.jqgufenzy.top

[Q90] 生成序号列
来源：http://fsg.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oly.guannengcc.top

================================================================================
来源：http://oka.cheryme.top

R. Bash 专题
来源：http://tlw.gotoacloud.top

================================================================================
来源：http://prz.cheryme.top

[R01] shebang 与严格模式
来源：http://lvp.hcnkem.com

#!/usr/bin/env bash
来源：http://rvk.snrcjt.cn

set -euo pipefail
来源：http://fjr.hammf.cn

[R02] 变量赋值与使用
来源：http://jzt.hcnkem.com

name="Tom"; echo "$name"
来源：http://uep.yuanzhike.top

[R03] 只读变量
来源：http://scu.yuanzhike.top

readonly PI=3.14
来源：http://oni.yfazqb.com

[R04] 位置参数
来源：http://dnh.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dmz.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://gbz.bbcook.cn

name="${1:-default}"
来源：http://dvd.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://pnm.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lnh.hongshengwenyu.top

[R07] if 判断文件
来源：http://vta.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jau.yueranfly.top

[R08] 数值比较
来源：http://ors.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oxz.gotoacloud.top

[R09] 字符串比较
来源：http://pip.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gnk.cqqwz.cn

[R10] 正则匹配
来源：http://bsf.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hlq.jiagoushi.top

[R11] case 多分支
来源：http://suw.yj20258888.top

case "$1" in
来源：http://tea.bbcook.cn

start) echo "启动" ;;
来源：http://ziz.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://ucr.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://nkv.zhoulong.xyz

esac
来源：http://qmw.fktsv.cn

[R12] for 遍历文件
来源：http://lcy.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://rdj.xuanzx.com

[R13] for 计数循环
来源：http://wkb.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://kgr.sysykeji.top

[R14] C 风格 for
来源：http://fzz.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pdn.hammf.cn

[R15] while 逐行读文件
来源：http://qjw.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mby.cashguo.top

[R16] until 等待条件
来源：http://daw.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zkn.bbcook.cn

[R17] 数组定义与取值
来源：http://unn.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://zpv.iojbl.cn

[R18] 遍历数组
来源：http://osu.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ljx.pycfn.com

[R19] 数组长度
来源：http://jyb.tianlin.xyz

echo "${#arr[@]}"
来源：http://sjs.ivvv.top

[R20] 关联数组（字典）
来源：http://cdy.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://stz.ehwqpu.com

[R21] 字符串长度
来源：http://czn.zhixingplan.top

echo "${#s}"
来源：http://qoa.tian-w.cn

[R22] 截取子串
来源：http://nbw.zhengqikj.top

echo "${s:0:5}"
来源：http://zag.yueranfly.top

[R23] 字符串替换
来源：http://kou.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eur.hesvh.cn

[R24] 大小写转换
来源：http://klq.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://mkv.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://baw.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://onw.yj202588.top

[R26] 命令替换
来源：http://tsv.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://rrt.yfazqb.com

[R27] 算术展开
来源：http://cdn.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://ohn.ivvv.top

[R28] 浮点运算
来源：http://ies.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://vtv.hnqzz.top

[R29] 定义函数
来源：http://nhj.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dme.mhx1999.top

[R30] 函数返回状态码
来源：http://dsx.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://izj.zdbjq.cn

[R31] 局部变量
来源：http://vgk.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://tgd.guannengcc.top

[R32] 参数个数校验
来源：http://hbp.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zbk.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://ses.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tgv.chenjidiqi.icu

[R34] 退出时清理
来源：http://dpj.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://szd.pycfn.com

[R35] 后台执行并等待
来源：http://ltg.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://prj.nanxinkj.top

[R36] 并发执行多个任务
来源：http://hby.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aim.yuxming.cn

[R37] 把输出赋给变量
来源：http://mcx.yonumen.top

files=$(ls -1)
来源：http://rtq.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://ztu.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://oyc.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://yja.dianchejie.cn

cmd > out.log 2>&1
来源：http://rli.ctjpmb.com

[R40] 追加写日志
来源：http://fnk.sjlbkw.cn

echo "log" >> out.log
来源：http://ial.fktsv.cn

[R41] 丢弃输出
来源：http://ifb.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://dxl.kuanghao11.cn

[R42] 输入重定向
来源：http://plr.nwbrower.top

wc -l < a.txt
来源：http://wsx.quarkkingdee.top

[R43] 按名字查找文件
来源：http://xwn.yj20258888.top

find . -name "*.log" -type f
来源：http://rno.tanke756.top

[R44] 按修改时间查找
来源：http://ooo.zhoulong.xyz

find . -mtime -7 -type f
来源：http://zxg.pengpengdd.cyou

[R45] 批量删除
来源：http://new.yvedp.cn

find . -name "*.tmp" -delete
来源：http://map.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://slb.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uvr.yanxiufei.cn

[R47] sed 单行替换
来源：http://arv.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xqg.haohaochexian.top

[R48] awk 取指定列
来源：http://dxe.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://ijh.xuetiantiany.cn

[R49] awk 带条件
来源：http://tha.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ywb.ctjpmb.com

[R50] awk 求和
来源：http://yga.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://tax.yanxiufei.cn

[R51] 排序去重取前几
来源：http://epk.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pmd.yj20258.top

[R52] 统计行数
来源：http://qhv.fanxiaobao.xyz

wc -l a.txt
来源：http://otn.ivvv.top

[R53] 查看文件头与实时尾
来源：http://spc.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://use.shangyingyoupin.top

[R54] 比较两个文件
来源：http://hsi.xuanzx.com

diff a.txt b.txt
来源：http://trv.hnxiangtu.top

[R55] 压缩与解压
来源：http://baa.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zoi.jlsjyb.cn

[R56] 远程拷贝
来源：http://cjj.ehwqpu.com

scp file user@host:/path/
来源：http://jzm.uphjek.com

[R57] 远程执行命令
来源：http://dox.yuxming.cn

ssh user@host 'uptime'
来源：http://wqo.epnwcf.com

[R58] 下载文件
来源：http://tfh.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ofd.nanxinkj.top

[R59] 发 POST JSON
来源：http://yke.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://btz.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://ekp.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cyo.cheryme.top

[R61] 磁盘占用
来源：http://ncu.xylfe.cn

df -h;  du -sh *
来源：http://ygr.hammf.cn

[R62] 找最占空间的文件
来源：http://jml.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://gza.nanxinkj.top

[R63] 内存与进程
来源：http://ejk.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://pll.sjlbkw.cn

[R64] 结束进程
来源：http://sfd.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://hyd.cucudq.cn

[R65] 查看端口占用
来源：http://viq.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://crk.zdqjudy.top

[R66] 定时任务
来源：http://ykm.jlsjyb.cn

crontab -e;  crontab -l
来源：http://opp.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://sko.jiagoushi.top

openssl rand -hex 16
来源：http://htf.sjlbkw.cn

[R68] 计算文件校验值
来源：http://szs.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aqr.smart0.xyz

[R69] 生成随机密码
来源：http://msp.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://xqs.jinqigfzy.top

[R70] 时间戳与互转
来源：http://jfh.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://zpj.sweek.top

[R71] 日期格式化
来源：http://ydo.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://edk.smart0.xyz

[R72] 等待端口就绪
来源：http://fmq.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iit.jqgufenzy.top

[R73] 分割大日志
来源：http://kwj.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://aui.yuxming.cn

[R74] 批量重命名
来源：http://bcf.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mez.hnxiangtu.top

[R75] 导出环境变量
来源：http://rhl.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://mzz.pycfn.com

[R76] 使用临时文件
来源：http://mgo.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hdg.svipenyu.cn

[R77] 读取用户输入
来源：http://nxv.yanxiufei.cn

read -rp "请输入: " ans
来源：http://qza.wangdashe.top

[R78] 交互式菜单
来源：http://hmp.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vqa.fehbvm.com

[R79] 解析命令行选项
来源：http://ajd.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vgo.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://qyz.daxiang520.top

time ./run.sh
来源：http://dul.haohaochexian.top

================================================================================
来源：http://emk.epnwcf.com

S. C / C++ 专题
来源：http://qcy.birdmap.top

================================================================================
来源：http://ejx.xinyue.icu

[S01] C：Hello World
来源：http://gjw.zdqjudy.top

#include <stdio.h>
来源：http://usv.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lns.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://dni.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://vbn.cucudq.cn

[S03] C：读入整数
来源：http://etp.chenlongwang.top

int x; scanf("%d", &x);
来源：http://yfq.shzxlz.cn

[S04] C：字符串复制
来源：http://uhf.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mgr.zdqjudy.top

[S05] C：字符串长度
来源：http://gan.gaohongyu789.top

strlen(s)
来源：http://owu.yuxming.cn

[S06] C：字符串比较
来源：http://qdo.fzhhl.top

strcmp(a, b) == 0
来源：http://lsn.316326.xyz

[S07] C：数组遍历求和
来源：http://gvx.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jdt.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://sun.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mln.havefunace.top

[S09] C：结构体定义与初始化
来源：http://bfn.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utv.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://exl.sweek.top

int *p = &a;  *p = 5;
来源：http://wzu.yfazqb.com

[S11] C：逐行读文件
来源：http://hog.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://jbu.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sqx.yangfankeji.com

fclose(f);
来源：http://pql.tian-w.cn

[S12] C：写文件
来源：http://fdp.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qkt.havefunace.top

[S13] C：宏定义
来源：http://rwx.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rox.jinyuanbaomall.cn

[S14] C：枚举
来源：http://oph.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://uzz.nanxuanxn.top

[S15] C：类型转换
来源：http://tgv.jqgfzy.top

(double) a / b
来源：http://map.ydzc1.top

[S16] C：位操作置位
来源：http://pqj.316326.xyz

x |= (1 << 3);
来源：http://afn.tanke756.top

[S17] C：安全拼接字符串
来源：http://rli.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sky.tian-w.cn

[S18] C：命令行参数
来源：http://piq.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://gra.svipenyu.cn

[S19] C：快速排序
来源：http://gsq.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://ppl.shanyushiyangtech.top

[S20] C：二分查找
来源：http://mqh.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oko.zhixingplan.top

[S21] C：字符类别判断
来源：http://wmd.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cts.chenlongwang.top

[S22] C：字符串转数字
来源：http://dxi.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vkq.chenlongwang.top

[S23] C：随机数
来源：http://mew.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mgv.daxiang520.top

[S24] C：获取本地时间
来源：http://ddx.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lgl.yueranfly.top

[S25] C：内存拷贝
来源：http://iiq.tian-w.cn

memcpy(dst, src, n);
来源：http://hbi.nanxinkj.top

[S26] C：内存清零
来源：http://rur.hesvh.cn

memset(a, 0, sizeof a);
来源：http://cdq.c1oappe.top

[S27] C：定义常量
来源：http://jco.aibaodan.cn

const double PI = 3.14159;
来源：http://kla.zhiwuduotai.top

[S28] C：静态变量
来源：http://ihl.yfazqb.com

static int counter = 0;
来源：http://hjk.xinyue.icu

[S29] C：变参函数
来源：http://ppo.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tzl.ydzc1.top

[S30] C：头文件保护
来源：http://iqz.snrcjt.cn

#ifndef X_H
来源：http://cla.hysaishi.cn

#define X_H
来源：http://vtv.fzhhl.top

#endif
来源：http://rln.nanxinkj.top

[S31] C++：Hello World
来源：http://tql.cashguo.top

#include <iostream>
来源：http://tot.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://zxf.yongpay.top

[S32] C++：字符串
来源：http://tkg.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://amg.yueranfly.top

[S33] C++：vector 增删
来源：http://yks.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tjn.sxryk.cn

[S34] C++：遍历 vector
来源：http://hwc.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://jaf.xingfuxueyuan.xyz

[S35] C++：map
来源：http://gii.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dxm.pycfn.com

[S36] C++：unordered_map
来源：http://irw.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nzt.zhengqikj.top

[S37] C++：set
来源：http://etc.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nix.cqqwz.cn

[S38] C++：排序
来源：http://piq.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://glb.yonumen.top

[S39] C++：自定义比较器排序
来源：http://vxj.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ejo.jlsjyb.cn

[S40] C++：查找元素
来源：http://qrg.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ntq.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://ahn.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pww.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://xqk.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://nyl.ydzc1.top

[S43] C++：智能指针
来源：http://bsy.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://mkp.xylfe.cn

[S44] C++：引用传参
来源：http://vrx.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://imw.fktsv.cn

[S45] C++：lambda
来源：http://sow.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://pwi.zhixingplan.top

[S46] C++：函数模板
来源：http://usy.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yze.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://znp.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qzb.fktsv.cn

[S48] C++：逐行读文件
来源：http://gaz.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://jfw.epnwcf.com

while (std::getline(in, line)) { }
来源：http://ddf.zdbjq.cn

[S49] C++：写文件
来源：http://bog.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uwp.uphjek.com

[S50] C++：格式化数字
来源：http://rpw.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yuq.jianghu66.top

[S51] C++：显式类型转换
来源：http://bio.tarul.cn

static_cast<double>(a) / b
来源：http://dma.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://eao.sweek.top

int size() const noexcept { return n_; }
来源：http://xjx.bjfxy.top

[S53] C++：移动语义
来源：http://lbw.ivvv.top

std::vector<int> w = std::move(v);
来源：http://wai.yj20258.top

[S54] C++：异常处理
来源：http://fiv.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bvt.andypj.xyz

[S55] C++：结构化绑定
来源：http://pir.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pxa.bjfxy.top

[S56] C++：optional
来源：http://nlj.shanyushiyangtech.top


<!-- 参考信息 -->