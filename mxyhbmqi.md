代发 wailian999

[Q84] 去除首尾空格
来源：http://vtu.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://gnx.mhx1999.top

[Q85] 数值取整
来源：http://omx.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://agb.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://jbt.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uzv.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://psz.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xti.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://xww.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fae.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wcu.zycfv.cn

[Q89] 判断表是否存在
来源：http://luh.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://afd.cdnleiting.top

[Q90] 生成序号列
来源：http://dbj.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ohr.cashguo.top

================================================================================
来源：http://max.sweek.top

R. Bash 专题
来源：http://kty.xingfuxueyuan.xyz

================================================================================
来源：http://npw.yangfankeji.com

[R01] shebang 与严格模式
来源：http://urb.guannengcc.top

#!/usr/bin/env bash
来源：http://aod.xuetiantiany.cn

set -euo pipefail
来源：http://giu.zdqjudy.top

[R02] 变量赋值与使用
来源：http://iwv.yuxming.cn

name="Tom"; echo "$name"
来源：http://rxm.bbcook.cn

[R03] 只读变量
来源：http://wwn.yanxiufei.cn

readonly PI=3.14
来源：http://dvm.pycfn.com

[R04] 位置参数
来源：http://jsn.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kqu.zdbjq.cn

[R05] 参数默认值
来源：http://hvq.nwbrower.top

name="${1:-default}"
来源：http://rsr.yuanzhike.top

[R06] 判断命令是否存在
来源：http://nlt.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jjn.shuidangran.top

[R07] if 判断文件
来源：http://ldr.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wnq.svipenyu.cn

[R08] 数值比较
来源：http://fmz.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zxc.hcnkem.com

[R09] 字符串比较
来源：http://ydv.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mks.guannengcc.top

[R10] 正则匹配
来源：http://kxw.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://exf.jinqigufen.top

[R11] case 多分支
来源：http://kdq.hnqzz.top

case "$1" in
来源：http://iws.yanxiufei.cn

start) echo "启动" ;;
来源：http://puu.ctjpmb.com

stop)  echo "停止" ;;
来源：http://fns.jianghu66.top

*)     echo "未知命令" ;;
来源：http://thu.yangfankeji.com

esac
来源：http://xbv.52xcode.cn

[R12] for 遍历文件
来源：http://kkq.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://bvr.yj202588.top

[R13] for 计数循环
来源：http://fpu.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://wzl.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://ifk.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://scp.fzhhl.top

[R15] while 逐行读文件
来源：http://iln.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxv.smart0.xyz

[R16] until 等待条件
来源：http://hjb.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://euc.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://kfn.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://inn.daxiang520.top

[R18] 遍历数组
来源：http://ykq.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yrv.svipenyu.cn

[R19] 数组长度
来源：http://zow.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://mzt.hywenlv.cn

[R20] 关联数组（字典）
来源：http://wan.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lpp.c1oappe.top

[R21] 字符串长度
来源：http://uai.vehdjk.com

echo "${#s}"
来源：http://rto.xylfe.cn

[R22] 截取子串
来源：http://orw.gogol.net.cn

echo "${s:0:5}"
来源：http://drp.hysaishi.cn

[R23] 字符串替换
来源：http://ypj.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sao.nanxinkj.top

[R24] 大小写转换
来源：http://bym.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nvx.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://fcc.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://axi.zycfv.cn

[R26] 命令替换
来源：http://cdj.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://jeu.hfpthk.cn

[R27] 算术展开
来源：http://dxb.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://wof.52xcode.cn

[R28] 浮点运算
来源：http://rjs.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://lst.nanxuanxn.top

[R29] 定义函数
来源：http://gau.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pfu.fktsv.cn

[R30] 函数返回状态码
来源：http://xds.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://lvj.hfpthk.cn

[R31] 局部变量
来源：http://nmm.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://mhm.yueranfly.top

[R32] 参数个数校验
来源：http://mko.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xrn.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://iny.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xsb.hywenlv.cn

[R34] 退出时清理
来源：http://jha.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://soa.kuanghao11.cn

[R35] 后台执行并等待
来源：http://eyt.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aoj.sufxvd.cn

[R36] 并发执行多个任务
来源：http://pfz.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fff.gzhubu.top

[R37] 把输出赋给变量
来源：http://ppk.jqgfzy.top

files=$(ls -1)
来源：http://daq.zycfv.cn

[R38] 管道串联
来源：http://phw.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://rdr.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://ouy.zhijiandao.cn

cmd > out.log 2>&1
来源：http://dut.dianchejie.cn

[R40] 追加写日志
来源：http://bsk.fehbvm.com

echo "log" >> out.log
来源：http://ded.epnwcf.com

[R41] 丢弃输出
来源：http://hzh.bjfxy.top

cmd >/dev/null 2>&1
来源：http://krc.tanke756.top

[R42] 输入重定向
来源：http://bnk.pycfn.com

wc -l < a.txt
来源：http://bmp.hysaishi.cn

[R43] 按名字查找文件
来源：http://vkv.hysaishi.cn

find . -name "*.log" -type f
来源：http://vgo.ctjpmb.com

[R44] 按修改时间查找
来源：http://kev.cqqwz.cn

find . -mtime -7 -type f
来源：http://txr.ybcxt.top

[R45] 批量删除
来源：http://ksz.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://ldj.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://ebq.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hus.hnxiangtu.top

[R47] sed 单行替换
来源：http://brv.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://bth.nanxinkj.top

[R48] awk 取指定列
来源：http://rgd.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://qxo.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://lsd.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mnl.aibaodan.cn

[R50] awk 求和
来源：http://gsm.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pcu.guannengcc.top

[R51] 排序去重取前几
来源：http://uim.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gty.iojbl.cn

[R52] 统计行数
来源：http://qnz.jqgfzy.top

wc -l a.txt
来源：http://qyf.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://hby.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aiv.zdbjq.cn

[R54] 比较两个文件
来源：http://sjy.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://wpg.cqqwz.cn

[R55] 压缩与解压
来源：http://sys.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wbp.iojbl.cn

[R56] 远程拷贝
来源：http://mip.jinqigfzy.top

scp file user@host:/path/
来源：http://hyd.daria6918.cn

[R57] 远程执行命令
来源：http://uap.bjfxy.top

ssh user@host 'uptime'
来源：http://izr.fanxiaobao.xyz

[R58] 下载文件
来源：http://bgl.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bbz.c1oappe.top

[R59] 发 POST JSON
来源：http://jou.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rae.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://bmx.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vum.kuanghao11.cn

[R61] 磁盘占用
来源：http://abi.nanxinkj.top

df -h;  du -sh *
来源：http://bed.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://oqx.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://guh.yuxming.cn

[R63] 内存与进程
来源：http://pkl.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://ndr.zhiwuduotai.top

[R64] 结束进程
来源：http://ckv.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://nlo.zhiwuduotai.top

[R65] 查看端口占用
来源：http://yin.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://izp.andypj.xyz

[R66] 定时任务
来源：http://ozm.yuxming.cn

crontab -e;  crontab -l
来源：http://uhh.52xcode.cn

[R67] 生成随机十六进制串
来源：http://oje.aibaodan.cn

openssl rand -hex 16
来源：http://fph.yuanzhike.top

[R68] 计算文件校验值
来源：http://ost.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://mmy.zhiwuduotai.top

[R69] 生成随机密码
来源：http://xqh.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://zdc.daria6918.cn

[R70] 时间戳与互转
来源：http://xtk.daxiang520.top

date +%s;  date -d @1700000000
来源：http://xro.jqgfzy.top

[R71] 日期格式化
来源：http://mqh.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rih.sufxvd.cn

[R72] 等待端口就绪
来源：http://abu.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://did.hammf.cn

[R73] 分割大日志
来源：http://jrn.birdmap.top

split -l 1000 big.log part_
来源：http://zcd.redwolf501.top

[R74] 批量重命名
来源：http://xcd.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jds.yj20258888.top

[R75] 导出环境变量
来源：http://iti.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://kfv.zhongyouzk.top

[R76] 使用临时文件
来源：http://tpj.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kdm.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://wsm.kuanghao11.cn

read -rp "请输入: " ans
来源：http://hiy.shuidangran.top

[R78] 交互式菜单
来源：http://brf.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://bnz.yj20258.top

[R79] 解析命令行选项
来源：http://gtc.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vzq.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://xbj.chenjidiqi.icu

time ./run.sh
来源：http://ggw.zhijiandao.cn

================================================================================
来源：http://edr.hywenlv.cn

S. C / C++ 专题
来源：http://rpp.cdnleiting.top

================================================================================
来源：http://sce.hongshengwenyu.top

[S01] C：Hello World
来源：http://dgs.ctjpmb.com

#include <stdio.h>
来源：http://tzk.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ajb.wangdashe.top

[S02] C：变量与格式化输出
来源：http://avq.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://gji.sweek.top

[S03] C：读入整数
来源：http://oxa.zycfv.cn

int x; scanf("%d", &x);
来源：http://yfp.yuanzhike.top

[S04] C：字符串复制
来源：http://ibe.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://fbw.meibo888.top

[S05] C：字符串长度
来源：http://fjv.yonumen.top

strlen(s)
来源：http://mzm.chenjidiqi.icu

[S06] C：字符串比较
来源：http://mto.nwbrower.top

strcmp(a, b) == 0
来源：http://mwk.fengsongda.top

[S07] C：数组遍历求和
来源：http://riq.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tcj.hammf.cn

[S08] C：动态内存分配与释放
来源：http://jmq.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylg.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://udu.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ehq.daxiang520.top

[S10] C：指针与解引用
来源：http://ccf.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://tpy.yueranfly.top

[S11] C：逐行读文件
来源：http://qvj.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://loo.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uik.fehbvm.com

fclose(f);
来源：http://qbp.bjfxy.top

[S12] C：写文件
来源：http://juc.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qvy.zdbjq.cn

[S13] C：宏定义
来源：http://osm.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://feu.tanke756.top

[S14] C：枚举
来源：http://kqe.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://jda.svipenyu.cn

[S15] C：类型转换
来源：http://jum.cheryme.top

(double) a / b
来源：http://owp.316326.xyz

[S16] C：位操作置位
来源：http://tqo.yangfankeji.com

x |= (1 << 3);
来源：http://uhj.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://knb.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://znb.gogol.net.cn

[S18] C：命令行参数
来源：http://pdk.redwolf501.top

int main(int argc, char **argv)
来源：http://pry.bbcook.cn

[S19] C：快速排序
来源：http://lrx.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://ect.hammf.cn

[S20] C：二分查找
来源：http://xit.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hir.jyoumei.cn

[S21] C：字符类别判断
来源：http://phk.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bgm.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://ytz.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://rtt.jinghuilouyu.cn

[S23] C：随机数
来源：http://twz.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yfh.zycfv.cn

[S24] C：获取本地时间
来源：http://jfx.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nzg.pycfn.com

[S25] C：内存拷贝
来源：http://tlz.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://rxu.kuanghao11.cn

[S26] C：内存清零
来源：http://ymh.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://yus.zhiwuduotai.top

[S27] C：定义常量
来源：http://cvp.tarul.cn

const double PI = 3.14159;
来源：http://mvo.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://utt.jqgfzy.top

static int counter = 0;
来源：http://pjw.hesvh.cn

[S29] C：变参函数
来源：http://dvm.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rmf.jiagoushi.top

[S30] C：头文件保护
来源：http://vlo.ehwqpu.com

#ifndef X_H
来源：http://ftp.jyoumei.cn

#define X_H
来源：http://ryf.cheryme.top

#endif
来源：http://vqw.pengpengdd.cyou

[S31] C++：Hello World
来源：http://fud.tarul.cn

#include <iostream>
来源：http://iby.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://ryx.tian-w.cn

[S32] C++：字符串
来源：http://hhj.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://xua.yj20258888.top

[S33] C++：vector 增删
来源：http://amr.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sga.hnqzz.top

[S34] C++：遍历 vector
来源：http://mew.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://oks.daria6918.cn

[S35] C++：map
来源：http://puv.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pnf.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://kth.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ozj.epnwcf.com

[S37] C++：set
来源：http://pbc.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rbh.birdmap.top

[S38] C++：排序
来源：http://asi.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://yaj.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://fdk.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xxs.xinyue.icu

[S40] C++：查找元素
来源：http://aps.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://evy.dianchejie.cn

[S41] C++：类与构造函数
来源：http://lkb.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iyc.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://mdu.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://jtg.meibo888.top

[S43] C++：智能指针
来源：http://wvd.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://ife.gogol.net.cn

[S44] C++：引用传参
来源：http://vyf.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://jwt.fzhhl.top

[S45] C++：lambda
来源：http://hck.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://qvq.zycfv.cn

[S46] C++：函数模板
来源：http://yna.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kog.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://lfb.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qrj.yfazqb.com

[S48] C++：逐行读文件
来源：http://ldn.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://olw.fehbvm.com

while (std::getline(in, line)) { }
来源：http://ldk.yuxming.cn

[S49] C++：写文件
来源：http://utb.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xhj.zdbjq.cn

[S50] C++：格式化数字
来源：http://els.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ffz.wangdashe.top

[S51] C++：显式类型转换
来源：http://jur.yuanzhike.top

static_cast<double>(a) / b
来源：http://rhd.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://uud.316326.xyz

int size() const noexcept { return n_; }
来源：http://jpi.hfpthk.cn

[S53] C++：移动语义
来源：http://lqr.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://uxj.ivvv.top

[S54] C++：异常处理
来源：http://arj.gogol.net.cn


<!-- 参考信息 -->