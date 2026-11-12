代发 wailian999

[Q86] 读取 JSON 字段
来源：http://fks.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rxa.redwolf501.top

[Q87] JSON 字段做条件
来源：http://tns.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wzh.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://vxn.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ueh.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://abm.yj202588.top

[Q89] 判断表是否存在
来源：http://jrq.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tpg.316326.xyz

[Q90] 生成序号列
来源：http://dwn.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ktr.hfpthk.cn

================================================================================
来源：http://qqd.hfpthk.cn

R. Bash 专题
来源：http://wqt.shanyushiyangtech.top

================================================================================
来源：http://pub.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://ifz.gotoacloud.top

#!/usr/bin/env bash
来源：http://uyk.meibo888.top

set -euo pipefail
来源：http://kqi.9152youxi.cn

[R02] 变量赋值与使用
来源：http://pgn.epnwcf.com

name="Tom"; echo "$name"
来源：http://jgm.hfpthk.cn

[R03] 只读变量
来源：http://piz.gzhubu.top

readonly PI=3.14
来源：http://dgl.jqgufenzy.top

[R04] 位置参数
来源：http://xxl.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zhf.xylfe.cn

[R05] 参数默认值
来源：http://joo.ydjk.org.cn

name="${1:-default}"
来源：http://iov.chenlongwang.top

[R06] 判断命令是否存在
来源：http://ewj.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://adl.sweek.top

[R07] if 判断文件
来源：http://kdb.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnk.iojbl.cn

[R08] 数值比较
来源：http://hoh.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://usw.hongshengwenyu.top

[R09] 字符串比较
来源：http://phy.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qxf.316326.xyz

[R10] 正则匹配
来源：http://zdx.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://llz.nanxuanxn.top

[R11] case 多分支
来源：http://mzw.yfazqb.com

case "$1" in
来源：http://obs.tarul.cn

start) echo "启动" ;;
来源：http://iwd.jqgfzy.top

stop)  echo "停止" ;;
来源：http://iyi.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://pgj.0kj1m.cn

esac
来源：http://owj.havefunace.top

[R12] for 遍历文件
来源：http://zeo.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://zoa.yvedp.cn

[R13] for 计数循环
来源：http://ylq.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://gso.iojbl.cn

[R14] C 风格 for
来源：http://pwa.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lew.andypj.xyz

[R15] while 逐行读文件
来源：http://fnb.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yrc.nanxinkj.top

[R16] until 等待条件
来源：http://qlf.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qkd.vqdsnc.cn

[R17] 数组定义与取值
来源：http://ofz.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://zcb.jinghuilouyu.cn

[R18] 遍历数组
来源：http://miq.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mnw.jinghuilouyu.cn

[R19] 数组长度
来源：http://eke.epnwcf.com

echo "${#arr[@]}"
来源：http://twn.fengsongda.top

[R20] 关联数组（字典）
来源：http://wpe.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wzl.chenlongwang.top

[R21] 字符串长度
来源：http://xzu.yvedp.cn

echo "${#s}"
来源：http://qwd.ybcxt.top

[R22] 截取子串
来源：http://eho.jiagoushi.top

echo "${s:0:5}"
来源：http://wdc.pengpengdd.cyou

[R23] 字符串替换
来源：http://zvz.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wvi.aibaodan.cn

[R24] 大小写转换
来源：http://iiy.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ixg.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://rvj.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uth.sxryk.cn

[R26] 命令替换
来源：http://mrg.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://zea.jinqigufen.top

[R27] 算术展开
来源：http://jxe.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://hkr.fengsongda.top

[R28] 浮点运算
来源：http://kpl.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://dml.jyoumei.cn

[R29] 定义函数
来源：http://vtk.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hcr.sysykeji.top

[R30] 函数返回状态码
来源：http://ofs.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://tei.smart0.xyz

[R31] 局部变量
来源：http://eea.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://hvs.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://dyj.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xsf.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://may.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aab.chenjidiqi.icu

[R34] 退出时清理
来源：http://ugl.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://gmo.tanke756.top

[R35] 后台执行并等待
来源：http://sug.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ooj.zhengqikj.top

[R36] 并发执行多个任务
来源：http://mzn.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qyl.zhengqikj.top

[R37] 把输出赋给变量
来源：http://qju.feifeiyinyue.top

files=$(ls -1)
来源：http://hvq.316326.xyz

[R38] 管道串联
来源：http://iyi.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://uws.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://dyy.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://afg.nanxuanxn.top

[R40] 追加写日志
来源：http://soi.zhoulong.xyz

echo "log" >> out.log
来源：http://cdt.daxiang520.top

[R41] 丢弃输出
来源：http://mck.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://mle.tianlin.xyz

[R42] 输入重定向
来源：http://gqd.dashuyun.cn

wc -l < a.txt
来源：http://yee.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://jid.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://ofu.yj20258888.top

[R44] 按修改时间查找
来源：http://hfh.zhengqikj.top

find . -mtime -7 -type f
来源：http://skf.hongshengwenyu.top

[R45] 批量删除
来源：http://liq.hcnkem.com

find . -name "*.tmp" -delete
来源：http://qpo.fktsv.cn

[R46] 递归替换文件内容
来源：http://ikf.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dvp.hfpthk.cn

[R47] sed 单行替换
来源：http://gxi.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://wlc.ehwqpu.com

[R48] awk 取指定列
来源：http://scq.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://tjo.mhx1999.top

[R49] awk 带条件
来源：http://xms.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cyi.bbcook.cn

[R50] awk 求和
来源：http://ywf.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://wzx.yj20258.top

[R51] 排序去重取前几
来源：http://kun.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iyt.vqdsnc.cn

[R52] 统计行数
来源：http://vlc.hnqzz.top

wc -l a.txt
来源：http://yhy.tanke756.top

[R53] 查看文件头与实时尾
来源：http://vou.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hsa.uphjek.com

[R54] 比较两个文件
来源：http://obv.guowangkeji.top

diff a.txt b.txt
来源：http://xup.sjlbkw.cn

[R55] 压缩与解压
来源：http://xlq.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fcy.pengpengdd.cyou

[R56] 远程拷贝
来源：http://djq.zhengqikj.top

scp file user@host:/path/
来源：http://jus.yonumen.top

[R57] 远程执行命令
来源：http://xae.yueranfly.top

ssh user@host 'uptime'
来源：http://izg.birdmap.top

[R58] 下载文件
来源：http://jns.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://arv.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://rxo.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yzj.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://hhq.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://asr.ydjk.org.cn

[R61] 磁盘占用
来源：http://zyi.zhengqikj.top

df -h;  du -sh *
来源：http://toa.jianghu66.top

[R62] 找最占空间的文件
来源：http://zzl.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://kxb.andypj.xyz

[R63] 内存与进程
来源：http://vfr.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://cmn.jinqigufen.top

[R64] 结束进程
来源：http://txz.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://izy.c1oappe.top

[R65] 查看端口占用
来源：http://yqw.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://srs.cashguo.top

[R66] 定时任务
来源：http://sis.xinyue.icu

crontab -e;  crontab -l
来源：http://nou.havefunace.top

[R67] 生成随机十六进制串
来源：http://ljp.hongshengwenyu.top

openssl rand -hex 16
来源：http://wsp.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://bqo.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://wuh.316326.xyz

[R69] 生成随机密码
来源：http://cfg.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://vvm.guannengcc.top

[R70] 时间戳与互转
来源：http://lfr.meibo888.top

date +%s;  date -d @1700000000
来源：http://hrg.cdnleiting.top

[R71] 日期格式化
来源：http://frt.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gzh.zycfv.cn

[R72] 等待端口就绪
来源：http://isx.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kie.zhengqikj.top

[R73] 分割大日志
来源：http://mdo.chenzaomai.com

split -l 1000 big.log part_
来源：http://byj.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://nie.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wge.kuanghao11.cn

[R75] 导出环境变量
来源：http://nzm.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://hbs.ydzc1.top

[R76] 使用临时文件
来源：http://gif.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wty.xylfe.cn

[R77] 读取用户输入
来源：http://wuj.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://had.xylfe.cn

[R78] 交互式菜单
来源：http://que.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hgz.tarul.cn

[R79] 解析命令行选项
来源：http://kgt.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fvd.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://bzi.dashuyun.cn

time ./run.sh
来源：http://zor.bjfxy.top

================================================================================
来源：http://hic.hywenlv.cn

S. C / C++ 专题
来源：http://zoy.haohaochexian.top

================================================================================
来源：http://igl.chenjidiqi.icu

[S01] C：Hello World
来源：http://gzb.zhongyouzk.top

#include <stdio.h>
来源：http://dcn.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://izc.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://dky.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://xhj.zhoulong.xyz

[S03] C：读入整数
来源：http://ttw.cucudq.cn

int x; scanf("%d", &x);
来源：http://ich.quarkkingdee.top

[S04] C：字符串复制
来源：http://thr.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://bsx.shangyingyoupin.top

[S05] C：字符串长度
来源：http://tha.hysaishi.cn

strlen(s)
来源：http://cik.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://nsj.mhx1999.top

strcmp(a, b) == 0
来源：http://kyp.gotoacloud.top

[S07] C：数组遍历求和
来源：http://nzj.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pnn.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://yur.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jmd.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://mbo.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ncx.gaohongyu789.top

[S10] C：指针与解引用
来源：http://afv.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://pwr.yanxiufei.cn

[S11] C：逐行读文件
来源：http://fpd.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://sib.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jss.dashuyun.cn

fclose(f);
来源：http://uut.havefunace.top

[S12] C：写文件
来源：http://dez.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kuf.xylfe.cn

[S13] C：宏定义
来源：http://vmt.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lkr.yongpay.top

[S14] C：枚举
来源：http://uay.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://gxx.jinqigfzy.top

[S15] C：类型转换
来源：http://sjx.feifeiyinyue.top

(double) a / b
来源：http://hxk.hongshengwenyu.top

[S16] C：位操作置位
来源：http://jqw.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://mxq.fengsongda.top

[S17] C：安全拼接字符串
来源：http://nnm.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://skl.yj20258888.top

[S18] C：命令行参数
来源：http://rzx.snrcjt.cn

int main(int argc, char **argv)
来源：http://drc.tarul.cn

[S19] C：快速排序
来源：http://tcc.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://pns.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://qvx.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jzt.jiagoushi.top

[S21] C：字符类别判断
来源：http://yyw.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jgl.nanxinkj.top

[S22] C：字符串转数字
来源：http://ctw.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://tnx.yueranfly.top

[S23] C：随机数
来源：http://uaa.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://asw.uphjek.com

[S24] C：获取本地时间
来源：http://mur.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oey.yj202588.top

[S25] C：内存拷贝
来源：http://src.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://quq.ppjwa.cn

[S26] C：内存清零
来源：http://pyd.iojbl.cn

memset(a, 0, sizeof a);
来源：http://ohu.daria6918.cn

[S27] C：定义常量
来源：http://rll.tanke756.top

const double PI = 3.14159;
来源：http://zjq.xuanzx.com

[S28] C：静态变量
来源：http://dng.snrcjt.cn

static int counter = 0;
来源：http://vpd.iojbl.cn

[S29] C：变参函数
来源：http://juv.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ycx.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://spe.havefunace.top

#ifndef X_H
来源：http://cey.hcnkem.com

#define X_H
来源：http://vca.daria6918.cn

#endif
来源：http://yuk.quarkkingdee.top

[S31] C++：Hello World
来源：http://luz.tanke756.top

#include <iostream>
来源：http://kvg.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://qgp.gzhubu.top

[S32] C++：字符串
来源：http://teo.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://ycj.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://mmp.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://epx.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://vzt.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://hlw.yongpay.top

[S35] C++：map
来源：http://yvr.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ujb.hysaishi.cn

[S36] C++：unordered_map
来源：http://gtk.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kwl.dashuyun.cn

[S37] C++：set
来源：http://gef.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xzc.pengpengdd.cyou

[S38] C++：排序
来源：http://ydj.cheryme.top

std::sort(v.begin(), v.end());
来源：http://bld.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://hqz.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mmz.zhiwuduotai.top

[S40] C++：查找元素
来源：http://cra.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qiy.birdmap.top

[S41] C++：类与构造函数
来源：http://pkb.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oav.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://qfo.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://hia.ctjpmb.com

[S43] C++：智能指针
来源：http://xfg.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://glb.cdnleiting.top

[S44] C++：引用传参
来源：http://mcu.ivvv.top

void inc(int &x) { ++x; }
来源：http://hsy.fehbvm.com

[S45] C++：lambda
来源：http://uul.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tix.nanxuanxn.top

[S46] C++：函数模板
来源：http://ggr.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgz.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://ntg.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mzc.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://xrz.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ghr.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://kfk.yongpay.top

[S49] C++：写文件
来源：http://qoh.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jcq.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://mva.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qhv.pycfn.com

[S51] C++：显式类型转换
来源：http://prr.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://jja.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://aqs.ivvv.top

int size() const noexcept { return n_; }
来源：http://rvj.ybcxt.top

[S53] C++：移动语义
来源：http://ddl.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://fge.nwbrower.top

[S54] C++：异常处理
来源：http://zwc.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mhk.hysaishi.cn

[S55] C++：结构化绑定
来源：http://mkq.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cvy.birdmap.top

[S56] C++：optional
来源：http://ydy.sweek.top


<!-- 参考信息 -->