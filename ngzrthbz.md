代发 wailian999

[Q84] 去除首尾空格
来源：http://wui.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://vzk.shzxlz.cn

[Q85] 数值取整
来源：http://kul.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qbe.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://brf.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mln.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://nmz.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mni.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://bgp.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://msj.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qkg.havefunace.top

[Q89] 判断表是否存在
来源：http://ufe.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://phm.zycfv.cn

[Q90] 生成序号列
来源：http://gzm.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kne.ydzc1.top

================================================================================
来源：http://jbq.cucudq.cn

R. Bash 专题
来源：http://ydu.kuanghao11.cn

================================================================================
来源：http://nba.nwbrower.top

[R01] shebang 与严格模式
来源：http://qgx.316326.xyz

#!/usr/bin/env bash
来源：http://nbx.9152youxi.cn

set -euo pipefail
来源：http://jae.xuanzx.com

[R02] 变量赋值与使用
来源：http://wxs.jianghu66.top

name="Tom"; echo "$name"
来源：http://iso.gaohongyu789.top

[R03] 只读变量
来源：http://utu.hywenlv.cn

readonly PI=3.14
来源：http://zkc.guowangkeji.top

[R04] 位置参数
来源：http://cez.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvw.bjfxy.top

[R05] 参数默认值
来源：http://bvp.jyoumei.cn

name="${1:-default}"
来源：http://rlp.jinqigufen.top

[R06] 判断命令是否存在
来源：http://nex.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bja.yongpay.top

[R07] if 判断文件
来源：http://imh.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ztd.bbcook.cn

[R08] 数值比较
来源：http://qvd.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hgl.sjlbkw.cn

[R09] 字符串比较
来源：http://sez.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://imw.guannengcc.top

[R10] 正则匹配
来源：http://aya.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xox.ppjwa.cn

[R11] case 多分支
来源：http://zgp.wangdashe.top

case "$1" in
来源：http://itk.yonumen.top

start) echo "启动" ;;
来源：http://ahu.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://etv.316326.xyz

*)     echo "未知命令" ;;
来源：http://uao.yonumen.top

esac
来源：http://rag.hysaishi.cn

[R12] for 遍历文件
来源：http://iht.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://wwc.shzxlz.cn

[R13] for 计数循环
来源：http://umq.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ihi.316326.xyz

[R14] C 风格 for
来源：http://kjm.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kqc.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://xfo.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nje.bbcook.cn

[R16] until 等待条件
来源：http://kbo.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gyi.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://dty.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cqe.zycfv.cn

[R18] 遍历数组
来源：http://thk.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hmn.zhoulong.xyz

[R19] 数组长度
来源：http://fts.zhongyouzk.top

echo "${#arr[@]}"
来源：http://hxm.guannengcc.top

[R20] 关联数组（字典）
来源：http://fbs.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://syh.yanxiufei.cn

[R21] 字符串长度
来源：http://fnn.ppjwa.cn

echo "${#s}"
来源：http://qpk.aibaodan.cn

[R22] 截取子串
来源：http://wrr.hnxiangtu.top

echo "${s:0:5}"
来源：http://fkp.kuanghao11.cn

[R23] 字符串替换
来源：http://yua.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gbc.redwolf501.top

[R24] 大小写转换
来源：http://bld.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hyg.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://uux.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vrd.hcnkem.com

[R26] 命令替换
来源：http://xen.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://mgl.jinqigufen.top

[R27] 算术展开
来源：http://uzr.fzhhl.top

echo $((1 + 2 * 3))
来源：http://zlu.hfpthk.cn

[R28] 浮点运算
来源：http://jml.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://gdu.nanxuanxn.top

[R29] 定义函数
来源：http://fht.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imz.fehbvm.com

[R30] 函数返回状态码
来源：http://lnm.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://riu.ydzc1.top

[R31] 局部变量
来源：http://xel.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://srx.chenlongwang.top

[R32] 参数个数校验
来源：http://tnw.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyd.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://lht.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tuh.sxryk.cn

[R34] 退出时清理
来源：http://weu.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://anp.jianghu66.top

[R35] 后台执行并等待
来源：http://jro.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xgd.yfazqb.com

[R36] 并发执行多个任务
来源：http://mcn.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uac.svipenyu.cn

[R37] 把输出赋给变量
来源：http://nqu.hongshengwenyu.top

files=$(ls -1)
来源：http://hxd.nanxuanxn.top

[R38] 管道串联
来源：http://yol.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://htk.cashguo.top

[R39] 重定向标准输出与错误
来源：http://jga.xylfe.cn

cmd > out.log 2>&1
来源：http://bje.zdqjudy.top

[R40] 追加写日志
来源：http://hkf.vehdjk.com

echo "log" >> out.log
来源：http://gwd.316326.xyz

[R41] 丢弃输出
来源：http://qnd.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://jpi.iojbl.cn

[R42] 输入重定向
来源：http://bdn.aibaodan.cn

wc -l < a.txt
来源：http://hzk.snrcjt.cn

[R43] 按名字查找文件
来源：http://afo.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://gbb.sjlbkw.cn

[R44] 按修改时间查找
来源：http://jep.hnqzz.top

find . -mtime -7 -type f
来源：http://qvc.yj20258.top

[R45] 批量删除
来源：http://oqz.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://ydt.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://hph.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sly.smart0.xyz

[R47] sed 单行替换
来源：http://ybs.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ypc.ydzc1.top

[R48] awk 取指定列
来源：http://dxi.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://cth.jinqigfzy.top

[R49] awk 带条件
来源：http://rnr.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lal.zhongyouzk.top

[R50] awk 求和
来源：http://adj.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://mlm.chenzaomai.com

[R51] 排序去重取前几
来源：http://myl.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kcy.jinyuanbaomall.cn

[R52] 统计行数
来源：http://zoc.chenjidiqi.icu

wc -l a.txt
来源：http://jpy.tarul.cn

[R53] 查看文件头与实时尾
来源：http://gcz.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://onb.sweek.top

[R54] 比较两个文件
来源：http://ktr.dashuyun.cn

diff a.txt b.txt
来源：http://qnv.guowangkeji.top

[R55] 压缩与解压
来源：http://bnu.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mda.jiagoushi.top

[R56] 远程拷贝
来源：http://ofd.iojbl.cn

scp file user@host:/path/
来源：http://ldp.aizwys.cn

[R57] 远程执行命令
来源：http://vlj.dashuyun.cn

ssh user@host 'uptime'
来源：http://dmo.hesvh.cn

[R58] 下载文件
来源：http://ndo.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xpj.andypj.xyz

[R59] 发 POST JSON
来源：http://yln.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uxv.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://ovk.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rtx.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://skr.hysaishi.cn

df -h;  du -sh *
来源：http://mmb.316326.xyz

[R62] 找最占空间的文件
来源：http://gya.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://uio.shuidangran.top

[R63] 内存与进程
来源：http://jpg.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://noy.gzhubu.top

[R64] 结束进程
来源：http://gnq.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://zcb.sxryk.cn

[R65] 查看端口占用
来源：http://xct.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zyn.meibo888.top

[R66] 定时任务
来源：http://roc.tanke756.top

crontab -e;  crontab -l
来源：http://jgk.aizwys.cn

[R67] 生成随机十六进制串
来源：http://orf.nwbrower.top

openssl rand -hex 16
来源：http://jos.ppjwa.cn

[R68] 计算文件校验值
来源：http://cwt.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://aci.cdnleiting.top

[R69] 生成随机密码
来源：http://mhs.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://dno.jyoumei.cn

[R70] 时间戳与互转
来源：http://clz.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://wet.sxryk.cn

[R71] 日期格式化
来源：http://vqg.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://nyy.nwbrower.top

[R72] 等待端口就绪
来源：http://ulg.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esi.ybcxt.top

[R73] 分割大日志
来源：http://saq.jinqigufen.top

split -l 1000 big.log part_
来源：http://nvz.xylfe.cn

[R74] 批量重命名
来源：http://qvb.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nbv.hongshengwenyu.top

[R75] 导出环境变量
来源：http://fbi.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://xqg.jlsjyb.cn

[R76] 使用临时文件
来源：http://hqp.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zij.havefunace.top

[R77] 读取用户输入
来源：http://hvm.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://pfa.nwbrower.top

[R78] 交互式菜单
来源：http://jys.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://imc.iojbl.cn

[R79] 解析命令行选项
来源：http://kly.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://smb.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://inf.epnwcf.com

time ./run.sh
来源：http://jip.snrcjt.cn

================================================================================
来源：http://dtq.yfazqb.com

S. C / C++ 专题
来源：http://fum.ctjpmb.com

================================================================================
来源：http://yoi.fehbvm.com

[S01] C：Hello World
来源：http://hmg.cdnleiting.top

#include <stdio.h>
来源：http://nef.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hxv.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://hjr.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://qun.hesvh.cn

[S03] C：读入整数
来源：http://cmk.gotoacloud.top

int x; scanf("%d", &x);
来源：http://pnp.shzxlz.cn

[S04] C：字符串复制
来源：http://aev.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nke.ybcxt.top

[S05] C：字符串长度
来源：http://dup.havefunace.top

strlen(s)
来源：http://jxn.zhoulong.xyz

[S06] C：字符串比较
来源：http://uxm.xylfe.cn

strcmp(a, b) == 0
来源：http://qht.sysykeji.top

[S07] C：数组遍历求和
来源：http://wlv.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xec.cheryme.top

[S08] C：动态内存分配与释放
来源：http://rtj.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://suz.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://dtq.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://trh.zdbjq.cn

[S10] C：指针与解引用
来源：http://xyv.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://gad.yvedp.cn

[S11] C：逐行读文件
来源：http://rjg.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://qdt.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ldm.andypj.xyz

fclose(f);
来源：http://ciz.shuidangran.top

[S12] C：写文件
来源：http://xfm.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kfo.guannengcc.top

[S13] C：宏定义
来源：http://jvs.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dmx.yfazqb.com

[S14] C：枚举
来源：http://coq.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ndo.xziqi.cn

[S15] C：类型转换
来源：http://yfx.yueranfly.top

(double) a / b
来源：http://ues.dianchejie.cn

[S16] C：位操作置位
来源：http://qze.quarkkingdee.top

x |= (1 << 3);
来源：http://yfs.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://sjo.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://epj.daxiang520.top

[S18] C：命令行参数
来源：http://rls.dianchejie.cn

int main(int argc, char **argv)
来源：http://jle.pycfn.com

[S19] C：快速排序
来源：http://usy.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://ytu.hysaishi.cn

[S20] C：二分查找
来源：http://ucu.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vvl.cashguo.top

[S21] C：字符类别判断
来源：http://eaj.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zwp.hammf.cn

[S22] C：字符串转数字
来源：http://ecc.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://lkc.birdmap.top

[S23] C：随机数
来源：http://idu.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://fcb.birdmap.top

[S24] C：获取本地时间
来源：http://crz.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dkx.fzhhl.top

[S25] C：内存拷贝
来源：http://zwx.ybcxt.top

memcpy(dst, src, n);
来源：http://ezl.fengsongda.top

[S26] C：内存清零
来源：http://brz.epnwcf.com

memset(a, 0, sizeof a);
来源：http://kfo.sweek.top

[S27] C：定义常量
来源：http://nxl.hongshengwenyu.top

const double PI = 3.14159;
来源：http://asn.wangdashe.top

[S28] C：静态变量
来源：http://uwv.haohaochexian.top

static int counter = 0;
来源：http://kxv.vqdsnc.cn

[S29] C：变参函数
来源：http://snb.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdl.guannengcc.top

[S30] C：头文件保护
来源：http://bvr.gotoacloud.top

#ifndef X_H
来源：http://jpp.nanxinkj.top

#define X_H
来源：http://gnj.redwolf501.top

#endif
来源：http://wul.hysaishi.cn

[S31] C++：Hello World
来源：http://wky.feifeiyinyue.top

#include <iostream>
来源：http://rot.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://arw.nanxinkj.top

[S32] C++：字符串
来源：http://axt.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://ymr.kuanghao11.cn

[S33] C++：vector 增删
来源：http://uit.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://egj.wangdashe.top

[S34] C++：遍历 vector
来源：http://ghv.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://yhe.hongshengwenyu.top

[S35] C++：map
来源：http://pmk.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rvg.hcnkem.com

[S36] C++：unordered_map
来源：http://gpw.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://paz.ywan-chungtsiang.top

[S37] C++：set
来源：http://goz.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rcn.cqqwz.cn

[S38] C++：排序
来源：http://lsh.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://lor.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://unc.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jrh.cashguo.top

[S40] C++：查找元素
来源：http://jfe.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xfo.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://egl.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bke.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://vfl.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://ltq.yonumen.top

[S43] C++：智能指针
来源：http://jsv.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://mcz.uphjek.com

[S44] C++：引用传参
来源：http://zjq.vehdjk.com

void inc(int &x) { ++x; }
来源：http://uga.hnxiangtu.top

[S45] C++：lambda
来源：http://umr.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://hgr.bjfxy.top

[S46] C++：函数模板
来源：http://jha.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfu.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://rtd.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xlg.xuanzx.com

[S48] C++：逐行读文件
来源：http://pss.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://orb.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://xke.svipenyu.cn

[S49] C++：写文件
来源：http://ide.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://icn.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://tkg.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gkd.iojbl.cn

[S51] C++：显式类型转换
来源：http://jat.52xcode.cn

static_cast<double>(a) / b
来源：http://tex.meibo888.top

[S52] C++：const 与 noexcept
来源：http://wwi.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://vgy.guannengcc.top

[S53] C++：移动语义
来源：http://ebq.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://lsk.sufxvd.cn

[S54] C++：异常处理
来源：http://syh.ywan-chungtsiang.top


<!-- 参考信息 -->