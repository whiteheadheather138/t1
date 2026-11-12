代发 wailian999

[Q80] 字符串截取
来源：http://icc.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rtl.zhengqikj.top

[Q81] 字符串替换
来源：http://ncj.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vwr.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://ltf.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://crb.yfazqb.com

[Q83] 大小写转换
来源：http://jxg.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://clk.ehwqpu.com

[Q84] 去除首尾空格
来源：http://mvj.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://srn.smart0.xyz

[Q85] 数值取整
来源：http://xtd.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nzo.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://nnn.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vth.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://iyu.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dfo.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://lhy.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kgh.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vki.0kj1m.cn

[Q89] 判断表是否存在
来源：http://fzr.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ras.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://ocr.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://agy.zdqjudy.top

================================================================================
来源：http://uee.yj20258.top

R. Bash 专题
来源：http://iyo.zhongyouzk.top

================================================================================
来源：http://kmr.jinqigufen.top

[R01] shebang 与严格模式
来源：http://yfl.gotoacloud.top

#!/usr/bin/env bash
来源：http://uov.chenzaomai.com

set -euo pipefail
来源：http://beq.316326.xyz

[R02] 变量赋值与使用
来源：http://edw.andypj.xyz

name="Tom"; echo "$name"
来源：http://jqv.tarul.cn

[R03] 只读变量
来源：http://rya.iojbl.cn

readonly PI=3.14
来源：http://upr.xuetiantiany.cn

[R04] 位置参数
来源：http://nbw.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ikv.yueranfly.top

[R05] 参数默认值
来源：http://lhu.xuetiantiany.cn

name="${1:-default}"
来源：http://rvv.cdnleiting.top

[R06] 判断命令是否存在
来源：http://tjz.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oki.iojbl.cn

[R07] if 判断文件
来源：http://ctr.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rjf.pycfn.com

[R08] 数值比较
来源：http://yig.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yts.ctjpmb.com

[R09] 字符串比较
来源：http://pkm.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jiz.0kj1m.cn

[R10] 正则匹配
来源：http://jso.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://okw.cdnleiting.top

[R11] case 多分支
来源：http://ecw.jlsjyb.cn

case "$1" in
来源：http://bkg.ydjk.org.cn

start) echo "启动" ;;
来源：http://vua.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://rna.cucudq.cn

*)     echo "未知命令" ;;
来源：http://ass.sxryk.cn

esac
来源：http://uko.chenlongwang.top

[R12] for 遍历文件
来源：http://wcy.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://yiv.zhongyouzk.top

[R13] for 计数循环
来源：http://lio.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://vqo.yonumen.top

[R14] C 风格 for
来源：http://kid.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gsz.daxiang520.top

[R15] while 逐行读文件
来源：http://bvx.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dvy.hesvh.cn

[R16] until 等待条件
来源：http://til.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dhm.hfpthk.cn

[R17] 数组定义与取值
来源：http://fiu.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://omn.nwbrower.top

[R18] 遍历数组
来源：http://atc.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://naq.cucudq.cn

[R19] 数组长度
来源：http://nev.cashguo.top

echo "${#arr[@]}"
来源：http://kib.guannengcc.top

[R20] 关联数组（字典）
来源：http://kul.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vvf.uphjek.com

[R21] 字符串长度
来源：http://pha.guannengcc.top

echo "${#s}"
来源：http://yxm.dashuyun.cn

[R22] 截取子串
来源：http://jrn.hongshengwenyu.top

echo "${s:0:5}"
来源：http://nrv.sufxvd.cn

[R23] 字符串替换
来源：http://txu.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tun.ivvv.top

[R24] 大小写转换
来源：http://cka.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://hxz.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://wab.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nkz.sufxvd.cn

[R26] 命令替换
来源：http://hra.tarul.cn

now=$(date +%F); echo "$now"
来源：http://vec.quarkkingdee.top

[R27] 算术展开
来源：http://pxo.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://bbc.gotoacloud.top

[R28] 浮点运算
来源：http://fei.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://qkc.havefunace.top

[R29] 定义函数
来源：http://kfi.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lbu.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://ddj.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://ybz.hongshengwenyu.top

[R31] 局部变量
来源：http://anx.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://fwi.tanke756.top

[R32] 参数个数校验
来源：http://bln.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bom.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://moq.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ewt.hysaishi.cn

[R34] 退出时清理
来源：http://dnx.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://dfy.yj202588.top

[R35] 后台执行并等待
来源：http://hom.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zmy.fengsongda.top

[R36] 并发执行多个任务
来源：http://mly.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kzz.cqqwz.cn

[R37] 把输出赋给变量
来源：http://fnx.zycfv.cn

files=$(ls -1)
来源：http://dos.bbcook.cn

[R38] 管道串联
来源：http://gwe.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://twn.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://asi.ydzc1.top

cmd > out.log 2>&1
来源：http://kqv.iojbl.cn

[R40] 追加写日志
来源：http://rzc.meibo888.top

echo "log" >> out.log
来源：http://wxo.guannengcc.top

[R41] 丢弃输出
来源：http://muq.yfazqb.com

cmd >/dev/null 2>&1
来源：http://jik.chenlongwang.top

[R42] 输入重定向
来源：http://iln.ybcxt.top

wc -l < a.txt
来源：http://xxy.ppjwa.cn

[R43] 按名字查找文件
来源：http://sas.tian-w.cn

find . -name "*.log" -type f
来源：http://lzo.andypj.xyz

[R44] 按修改时间查找
来源：http://pyt.gzhubu.top

find . -mtime -7 -type f
来源：http://yhw.andypj.xyz

[R45] 批量删除
来源：http://wfc.zycfv.cn

find . -name "*.tmp" -delete
来源：http://tcb.bbcook.cn

[R46] 递归替换文件内容
来源：http://mkg.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qdh.dianchejie.cn

[R47] sed 单行替换
来源：http://poy.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://kyw.zhongyouzk.top

[R48] awk 取指定列
来源：http://eln.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://epw.daria6918.cn

[R49] awk 带条件
来源：http://zwo.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lrf.fengsongda.top

[R50] awk 求和
来源：http://yfg.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://utn.jyoumei.cn

[R51] 排序去重取前几
来源：http://mkl.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jys.nanxuanxn.top

[R52] 统计行数
来源：http://aqb.nwbrower.top

wc -l a.txt
来源：http://trn.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://edt.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gvf.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://rub.xinyue.icu

diff a.txt b.txt
来源：http://avq.hfpthk.cn

[R55] 压缩与解压
来源：http://xof.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yrm.pycfn.com

[R56] 远程拷贝
来源：http://pso.nanxinkj.top

scp file user@host:/path/
来源：http://ofj.yonumen.top

[R57] 远程执行命令
来源：http://xim.hnxiangtu.top

ssh user@host 'uptime'
来源：http://cjb.zhiwuduotai.top

[R58] 下载文件
来源：http://qzs.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lvd.ybcxt.top

[R59] 发 POST JSON
来源：http://hbv.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qoi.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://hea.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iqx.tarul.cn

[R61] 磁盘占用
来源：http://dlj.fktsv.cn

df -h;  du -sh *
来源：http://xvi.jqgfzy.top

[R62] 找最占空间的文件
来源：http://gon.ivvv.top

du -ah . | sort -rh | head -10
来源：http://ifm.hnqzz.top

[R63] 内存与进程
来源：http://sve.yj202588.top

free -h;  ps aux | grep nginx
来源：http://ege.zhoulong.xyz

[R64] 结束进程
来源：http://pre.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://hsr.dianchejie.cn

[R65] 查看端口占用
来源：http://nwx.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kij.dianchejie.cn

[R66] 定时任务
来源：http://hhv.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://gtz.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://yex.shanyushiyangtech.top

openssl rand -hex 16
来源：http://rwi.ctjpmb.com

[R68] 计算文件校验值
来源：http://bio.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://eru.pengpengdd.cyou

[R69] 生成随机密码
来源：http://dhc.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://byq.wangdashe.top

[R70] 时间戳与互转
来源：http://ukq.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://erk.chenzaomai.com

[R71] 日期格式化
来源：http://pmb.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qgo.hfpthk.cn

[R72] 等待端口就绪
来源：http://bzs.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bgk.xuanzx.com

[R73] 分割大日志
来源：http://ygq.jianghu66.top

split -l 1000 big.log part_
来源：http://pll.mhx1999.top

[R74] 批量重命名
来源：http://gip.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wcx.hammf.cn

[R75] 导出环境变量
来源：http://zsq.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://joo.shzxlz.cn

[R76] 使用临时文件
来源：http://gsn.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://imx.shangyingyoupin.top

[R77] 读取用户输入
来源：http://iyt.yj202588.top

read -rp "请输入: " ans
来源：http://wnn.zhengqikj.top

[R78] 交互式菜单
来源：http://elm.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tbn.yanxiufei.cn

[R79] 解析命令行选项
来源：http://bds.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uco.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://hiw.52xcode.cn

time ./run.sh
来源：http://mbu.tarul.cn

================================================================================
来源：http://vut.gzhubu.top

S. C / C++ 专题
来源：http://ajd.zdbjq.cn

================================================================================
来源：http://tou.pengpengdd.cyou

[S01] C：Hello World
来源：http://lfz.hysaishi.cn

#include <stdio.h>
来源：http://gdx.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hqx.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://nry.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://jvd.ctjpmb.com

[S03] C：读入整数
来源：http://mrj.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://epx.hfpthk.cn

[S04] C：字符串复制
来源：http://tst.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://gbc.yanxiufei.cn

[S05] C：字符串长度
来源：http://kvh.zhixingplan.top

strlen(s)
来源：http://vok.zhixingplan.top

[S06] C：字符串比较
来源：http://dkw.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://fqm.hcnkem.com

[S07] C：数组遍历求和
来源：http://szg.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pjl.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://ekw.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hrw.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://acp.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rps.zhixingplan.top

[S10] C：指针与解引用
来源：http://aiv.fktsv.cn

int *p = &a;  *p = 5;
来源：http://otu.hnqzz.top

[S11] C：逐行读文件
来源：http://wbe.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://vzc.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ktb.shangyingyoupin.top

fclose(f);
来源：http://iaf.jinqigufen.top

[S12] C：写文件
来源：http://zpn.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lqu.cheryme.top

[S13] C：宏定义
来源：http://jaw.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dgx.zhijiandao.cn

[S14] C：枚举
来源：http://dhx.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://utv.feifeiyinyue.top

[S15] C：类型转换
来源：http://xii.shzxlz.cn

(double) a / b
来源：http://rtm.redwolf501.top

[S16] C：位操作置位
来源：http://xdz.kuanghao11.cn

x |= (1 << 3);
来源：http://csn.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://vts.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uda.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://cnn.xziqi.cn

int main(int argc, char **argv)
来源：http://qmr.fktsv.cn

[S19] C：快速排序
来源：http://uau.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vuz.zhoulong.xyz

[S20] C：二分查找
来源：http://yna.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zfs.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://heh.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jyu.yanxiufei.cn

[S22] C：字符串转数字
来源：http://psd.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://xpt.zdbjq.cn

[S23] C：随机数
来源：http://bhx.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fjq.tian-w.cn

[S24] C：获取本地时间
来源：http://hcv.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yra.jinqigufen.top

[S25] C：内存拷贝
来源：http://tyt.ydzc1.top

memcpy(dst, src, n);
来源：http://sze.ppjwa.cn

[S26] C：内存清零
来源：http://aim.yj202588.top

memset(a, 0, sizeof a);
来源：http://ern.yfazqb.com

[S27] C：定义常量
来源：http://msl.xuetiantiany.cn

const double PI = 3.14159;
来源：http://tkk.cucudq.cn

[S28] C：静态变量
来源：http://tzi.bjfxy.top

static int counter = 0;
来源：http://tnk.yj202588.top

[S29] C：变参函数
来源：http://wsr.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hjk.zycfv.cn

[S30] C：头文件保护
来源：http://isq.vehdjk.com

#ifndef X_H
来源：http://czh.pycfn.com

#define X_H
来源：http://iyn.9152youxi.cn

#endif
来源：http://pho.gzhubu.top

[S31] C++：Hello World
来源：http://gqf.jiagoushi.top

#include <iostream>
来源：http://zth.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://tpk.zhoulong.xyz

[S32] C++：字符串
来源：http://igf.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://zvo.havefunace.top

[S33] C++：vector 增删
来源：http://att.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://upk.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://ijz.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vyd.zdbjq.cn

[S35] C++：map
来源：http://ldc.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ypc.dianchejie.cn

[S36] C++：unordered_map
来源：http://suk.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bzt.ywan-chungtsiang.top

[S37] C++：set
来源：http://syn.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbm.iojbl.cn

[S38] C++：排序
来源：http://hxt.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://gpu.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://icq.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ibq.zycfv.cn

[S40] C++：查找元素
来源：http://npd.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uwe.yvedp.cn

[S41] C++：类与构造函数
来源：http://blt.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ltl.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://tdr.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://lst.gaohongyu789.top

[S43] C++：智能指针
来源：http://vxw.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://scq.hongshengwenyu.top

[S44] C++：引用传参
来源：http://cst.pycfn.com

void inc(int &x) { ++x; }
来源：http://taf.yuanzhike.top

[S45] C++：lambda
来源：http://dft.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vbp.gotoacloud.top

[S46] C++：函数模板
来源：http://tfr.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://unq.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://kop.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tht.xylfe.cn

[S48] C++：逐行读文件
来源：http://lyo.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lwx.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://cky.yj20258888.top

[S49] C++：写文件
来源：http://aev.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zvr.zhongyouzk.top

[S50] C++：格式化数字
来源：http://dgv.xziqi.cn


<!-- 参考信息 -->