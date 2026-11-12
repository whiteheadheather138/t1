代发 wailian999

[Q86] 读取 JSON 字段
来源：http://maa.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fdd.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://vct.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://miz.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://uiw.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://olc.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ejr.gzhubu.top

[Q89] 判断表是否存在
来源：http://szb.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xqv.cdnleiting.top

[Q90] 生成序号列
来源：http://alc.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gpk.ehwqpu.com

================================================================================
来源：http://ssn.yueranfly.top

R. Bash 专题
来源：http://dcd.gotoacloud.top

================================================================================
来源：http://iaw.ivvv.top

[R01] shebang 与严格模式
来源：http://sxw.tian-w.cn

#!/usr/bin/env bash
来源：http://dxr.jinyuanbaomall.cn

set -euo pipefail
来源：http://dgp.yj20258888.top

[R02] 变量赋值与使用
来源：http://geg.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://nbs.cucudq.cn

[R03] 只读变量
来源：http://pwu.zdqjudy.top

readonly PI=3.14
来源：http://fyj.ppjwa.cn

[R04] 位置参数
来源：http://bbt.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ftq.9152youxi.cn

[R05] 参数默认值
来源：http://jhh.zhengqikj.top

name="${1:-default}"
来源：http://uuh.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://ivq.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://flo.bjfxy.top

[R07] if 判断文件
来源：http://owe.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://imn.yongpay.top

[R08] 数值比较
来源：http://fmm.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oov.tian-w.cn

[R09] 字符串比较
来源：http://bqj.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jwz.jyoumei.cn

[R10] 正则匹配
来源：http://zfa.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bho.jqgufenzy.top

[R11] case 多分支
来源：http://net.jyoumei.cn

case "$1" in
来源：http://ppq.yuxming.cn

start) echo "启动" ;;
来源：http://wuu.gotoacloud.top

stop)  echo "停止" ;;
来源：http://qmu.tian-w.cn

*)     echo "未知命令" ;;
来源：http://tye.yj202588.top

esac
来源：http://zhg.gaohongyu789.top

[R12] for 遍历文件
来源：http://itp.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://mut.xziqi.cn

[R13] for 计数循环
来源：http://tsu.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://bfu.hnqzz.top

[R14] C 风格 for
来源：http://sqr.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mgb.hfpthk.cn

[R15] while 逐行读文件
来源：http://bxb.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eyp.9152youxi.cn

[R16] until 等待条件
来源：http://guz.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rcd.yj20258.top

[R17] 数组定义与取值
来源：http://nuy.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ymh.aizwys.cn

[R18] 遍历数组
来源：http://tbn.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://duh.hnxiangtu.top

[R19] 数组长度
来源：http://gxb.nanxuanxn.top

echo "${#arr[@]}"
来源：http://gsd.birdmap.top

[R20] 关联数组（字典）
来源：http://buz.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bsp.haohaochexian.top

[R21] 字符串长度
来源：http://pmr.yueranfly.top

echo "${#s}"
来源：http://mqc.yvedp.cn

[R22] 截取子串
来源：http://yaw.fehbvm.com

echo "${s:0:5}"
来源：http://erc.xuanzx.com

[R23] 字符串替换
来源：http://yuc.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mxj.cqqwz.cn

[R24] 大小写转换
来源：http://loe.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wrz.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://hcp.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://otn.wangdashe.top

[R26] 命令替换
来源：http://irx.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://pwp.c1oappe.top

[R27] 算术展开
来源：http://ath.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://mqe.shanyushiyangtech.top

[R28] 浮点运算
来源：http://pxo.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://eqv.pengpengdd.cyou

[R29] 定义函数
来源：http://bgl.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://csi.zhijiandao.cn

[R30] 函数返回状态码
来源：http://sim.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://qij.hfpthk.cn

[R31] 局部变量
来源：http://roa.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://tez.chenzaomai.com

[R32] 参数个数校验
来源：http://pyv.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://trj.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://gpn.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kgw.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://mgp.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ufx.sysykeji.top

[R35] 后台执行并等待
来源：http://xgo.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dje.ehwqpu.com

[R36] 并发执行多个任务
来源：http://gyy.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wmx.gogol.net.cn

[R37] 把输出赋给变量
来源：http://afi.hfpthk.cn

files=$(ls -1)
来源：http://usk.cheryme.top

[R38] 管道串联
来源：http://gqo.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://shp.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://wno.haohaochexian.top

cmd > out.log 2>&1
来源：http://tdv.yanxiufei.cn

[R40] 追加写日志
来源：http://nmg.nwbrower.top

echo "log" >> out.log
来源：http://csf.gogol.net.cn

[R41] 丢弃输出
来源：http://xib.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://apa.316326.xyz

[R42] 输入重定向
来源：http://iva.pycfn.com

wc -l < a.txt
来源：http://nrj.cdnleiting.top

[R43] 按名字查找文件
来源：http://ade.sysykeji.top

find . -name "*.log" -type f
来源：http://ags.haohaochexian.top

[R44] 按修改时间查找
来源：http://dzv.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://tso.jiagoushi.top

[R45] 批量删除
来源：http://vnh.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://wcx.ehwqpu.com

[R46] 递归替换文件内容
来源：http://hld.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yuc.hesvh.cn

[R47] sed 单行替换
来源：http://xcd.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://cuk.yueranfly.top

[R48] awk 取指定列
来源：http://auj.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://pdp.jinqigufen.top

[R49] awk 带条件
来源：http://woo.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qia.feifeiyinyue.top

[R50] awk 求和
来源：http://nyv.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://rbg.vqdsnc.cn

[R51] 排序去重取前几
来源：http://kam.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://uju.andypj.xyz

[R52] 统计行数
来源：http://sjt.bjfxy.top

wc -l a.txt
来源：http://frz.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://ifv.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zsb.dashuyun.cn

[R54] 比较两个文件
来源：http://qyo.hongshengwenyu.top

diff a.txt b.txt
来源：http://bzl.sjlbkw.cn

[R55] 压缩与解压
来源：http://gnc.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://drd.yj20258.top

[R56] 远程拷贝
来源：http://nkx.chenzaomai.com

scp file user@host:/path/
来源：http://wwk.pengpengdd.cyou

[R57] 远程执行命令
来源：http://zpf.yvedp.cn

ssh user@host 'uptime'
来源：http://oyq.ppjwa.cn

[R58] 下载文件
来源：http://qfs.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gsh.c1oappe.top

[R59] 发 POST JSON
来源：http://qes.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nwj.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://jvz.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ajn.aibaodan.cn

[R61] 磁盘占用
来源：http://ovg.yvedp.cn

df -h;  du -sh *
来源：http://egm.yj20258.top

[R62] 找最占空间的文件
来源：http://amo.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://qzv.zhiwuduotai.top

[R63] 内存与进程
来源：http://gsh.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://cvz.quarkkingdee.top

[R64] 结束进程
来源：http://xak.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://phr.52xcode.cn

[R65] 查看端口占用
来源：http://kcb.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uln.cheryme.top

[R66] 定时任务
来源：http://rek.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://pav.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://lla.ehwqpu.com

openssl rand -hex 16
来源：http://clm.gaohongyu789.top

[R68] 计算文件校验值
来源：http://jbo.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nma.pengpengdd.cyou

[R69] 生成随机密码
来源：http://uwj.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://ecg.tian-w.cn

[R70] 时间戳与互转
来源：http://xnx.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://buj.wangshuangyany.cn

[R71] 日期格式化
来源：http://vrj.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybu.kuanghao11.cn

[R72] 等待端口就绪
来源：http://rgp.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ycs.bjfxy.top

[R73] 分割大日志
来源：http://lhx.gogol.net.cn

split -l 1000 big.log part_
来源：http://ooo.c1oappe.top

[R74] 批量重命名
来源：http://mxf.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xkm.guowangkeji.top

[R75] 导出环境变量
来源：http://ghi.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://rtq.tianlin.xyz

[R76] 使用临时文件
来源：http://ide.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uoc.hesvh.cn

[R77] 读取用户输入
来源：http://kwc.nanxinkj.top

read -rp "请输入: " ans
来源：http://jfp.hfpthk.cn

[R78] 交互式菜单
来源：http://ofj.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://mfa.chenlongwang.top

[R79] 解析命令行选项
来源：http://itq.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aby.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://wjo.xuanzx.com

time ./run.sh
来源：http://ysy.wangdashe.top

================================================================================
来源：http://jai.ctjpmb.com

S. C / C++ 专题
来源：http://cez.vehdjk.com

================================================================================
来源：http://nii.sjlbkw.cn

[S01] C：Hello World
来源：http://xjb.guowangkeji.top

#include <stdio.h>
来源：http://nau.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fcd.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://dyg.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://myw.shuidangran.top

[S03] C：读入整数
来源：http://yus.havefunace.top

int x; scanf("%d", &x);
来源：http://voi.yj20258888.top

[S04] C：字符串复制
来源：http://wke.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://icz.zhoulong.xyz

[S05] C：字符串长度
来源：http://vqs.yangfankeji.com

strlen(s)
来源：http://ggk.birdmap.top

[S06] C：字符串比较
来源：http://vrt.ppjwa.cn

strcmp(a, b) == 0
来源：http://mgu.bbcook.cn

[S07] C：数组遍历求和
来源：http://vow.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rup.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://nak.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zgo.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://akd.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://knx.zhengqikj.top

[S10] C：指针与解引用
来源：http://wxt.sysykeji.top

int *p = &a;  *p = 5;
来源：http://uzp.cqqwz.cn

[S11] C：逐行读文件
来源：http://mre.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://qwv.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jqh.bbcook.cn

fclose(f);
来源：http://jop.jyoumei.cn

[S12] C：写文件
来源：http://kuv.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://llq.hcnkem.com

[S13] C：宏定义
来源：http://bdg.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ibv.birdmap.top

[S14] C：枚举
来源：http://eas.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://uhq.yonumen.top

[S15] C：类型转换
来源：http://ujl.gotoacloud.top

(double) a / b
来源：http://eys.quarkkingdee.top

[S16] C：位操作置位
来源：http://btc.redwolf501.top

x |= (1 << 3);
来源：http://edl.52xcode.cn

[S17] C：安全拼接字符串
来源：http://jdg.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://esn.fzhhl.top

[S18] C：命令行参数
来源：http://usu.gaohongyu789.top

int main(int argc, char **argv)
来源：http://gwc.jqgufenzy.top

[S19] C：快速排序
来源：http://gmd.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://qjj.quarkkingdee.top

[S20] C：二分查找
来源：http://szl.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kmq.xziqi.cn

[S21] C：字符类别判断
来源：http://hcc.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfm.nanxinkj.top

[S22] C：字符串转数字
来源：http://rui.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://afs.yj20258888.top

[S23] C：随机数
来源：http://ofr.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ydb.xuanzx.com

[S24] C：获取本地时间
来源：http://wmg.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://glh.sysykeji.top

[S25] C：内存拷贝
来源：http://sxr.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://qje.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://ojm.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://gwy.ivvv.top

[S27] C：定义常量
来源：http://kst.jinqigufen.top

const double PI = 3.14159;
来源：http://mkd.wangshuangyany.cn

[S28] C：静态变量
来源：http://uma.haohaochexian.top

static int counter = 0;
来源：http://kdf.yj20258.top

[S29] C：变参函数
来源：http://xou.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fey.smart0.xyz

[S30] C：头文件保护
来源：http://dgy.yj202588.top

#ifndef X_H
来源：http://moe.quarkkingdee.top

#define X_H
来源：http://woo.jiagoushi.top

#endif
来源：http://vyx.yangfankeji.com

[S31] C++：Hello World
来源：http://qaa.kuanghao11.cn

#include <iostream>
来源：http://daz.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://wlq.sjlbkw.cn

[S32] C++：字符串
来源：http://pby.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://fbm.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://ows.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ztt.jqgfzy.top

[S34] C++：遍历 vector
来源：http://xsr.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://wku.andypj.xyz

[S35] C++：map
来源：http://hsf.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lyz.chenzaomai.com

[S36] C++：unordered_map
来源：http://tle.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lfi.hammf.cn

[S37] C++：set
来源：http://pfp.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lix.sufxvd.cn

[S38] C++：排序
来源：http://zsk.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://jdr.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://nvz.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cdf.gzhubu.top

[S40] C++：查找元素
来源：http://jma.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jvf.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://pdi.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bxx.yvedp.cn

[S42] C++：继承与虚函数
来源：http://nfm.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://vmo.andypj.xyz

[S43] C++：智能指针
来源：http://cmz.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://iyv.xziqi.cn

[S44] C++：引用传参
来源：http://yju.bjfxy.top

void inc(int &x) { ++x; }
来源：http://icq.shanyushiyangtech.top

[S45] C++：lambda
来源：http://wgq.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jmm.sxryk.cn

[S46] C++：函数模板
来源：http://ojv.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kza.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://bbl.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqe.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://ori.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://rhl.yvedp.cn

while (std::getline(in, line)) { }
来源：http://nuh.yvedp.cn

[S49] C++：写文件
来源：http://cix.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://imt.xuanzx.com

[S50] C++：格式化数字
来源：http://fvt.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://onl.shzxlz.cn

[S51] C++：显式类型转换
来源：http://hin.sxryk.cn

static_cast<double>(a) / b
来源：http://bbo.yj202588.top

[S52] C++：const 与 noexcept
来源：http://plj.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://ojn.52xcode.cn

[S53] C++：移动语义
来源：http://qdp.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://oqb.jianghu66.top

[S54] C++：异常处理
来源：http://hcd.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bon.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://vqz.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://req.hcnkem.com

[S56] C++：optional
来源：http://jwn.sysykeji.top


<!-- 参考信息 -->