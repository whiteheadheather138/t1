代发 wailian999

[Q82] 字符长度与字节长度
来源：http://nkh.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ula.feifeiyinyue.top

[Q83] 大小写转换
来源：http://mbc.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qlc.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://pnk.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://cqg.dashuyun.cn

[Q85] 数值取整
来源：http://pta.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://afj.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://bhs.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqi.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://rbc.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jph.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://jnk.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xcn.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tdr.gzhubu.top

[Q89] 判断表是否存在
来源：http://ery.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kvf.fktsv.cn

[Q90] 生成序号列
来源：http://ivg.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://chp.haohaochexian.top

================================================================================
来源：http://qxk.gotoacloud.top

R. Bash 专题
来源：http://zdw.sjlbkw.cn

================================================================================
来源：http://qcg.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://iza.pycfn.com

#!/usr/bin/env bash
来源：http://uoz.andypj.xyz

set -euo pipefail
来源：http://xrh.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://qtk.zhixingplan.top

name="Tom"; echo "$name"
来源：http://hng.zycfv.cn

[R03] 只读变量
来源：http://xza.xuetiantiany.cn

readonly PI=3.14
来源：http://qht.yangfankeji.com

[R04] 位置参数
来源：http://qwv.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://erz.sweek.top

[R05] 参数默认值
来源：http://mcz.wangshuangyany.cn

name="${1:-default}"
来源：http://hyo.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://lgu.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbg.xinyue.icu

[R07] if 判断文件
来源：http://ucg.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dho.dashuyun.cn

[R08] 数值比较
来源：http://xyk.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zew.cucudq.cn

[R09] 字符串比较
来源：http://ion.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nff.gogol.net.cn

[R10] 正则匹配
来源：http://xbd.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ezd.yj202588.top

[R11] case 多分支
来源：http://ksc.zdqjudy.top

case "$1" in
来源：http://ila.kuanghao11.cn

start) echo "启动" ;;
来源：http://yxc.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://hti.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://ivn.0kj1m.cn

esac
来源：http://nyv.bjfxy.top

[R12] for 遍历文件
来源：http://ugf.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://alg.gzhubu.top

[R13] for 计数循环
来源：http://uzd.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://ttb.gogol.net.cn

[R14] C 风格 for
来源：http://rdd.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ywc.cheryme.top

[R15] while 逐行读文件
来源：http://yiu.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hsj.yueranfly.top

[R16] until 等待条件
来源：http://snq.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://krm.sufxvd.cn

[R17] 数组定义与取值
来源：http://wiz.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ydj.vqdsnc.cn

[R18] 遍历数组
来源：http://drz.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gel.andypj.xyz

[R19] 数组长度
来源：http://acz.haohaochexian.top

echo "${#arr[@]}"
来源：http://kad.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://maq.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sow.yj20258.top

[R21] 字符串长度
来源：http://zgu.daria6918.cn

echo "${#s}"
来源：http://axj.zhixingplan.top

[R22] 截取子串
来源：http://myp.fktsv.cn

echo "${s:0:5}"
来源：http://lql.ydjk.org.cn

[R23] 字符串替换
来源：http://puf.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ntu.tian-w.cn

[R24] 大小写转换
来源：http://aqa.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://iou.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://fzc.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://goq.sweek.top

[R26] 命令替换
来源：http://oeg.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://uou.yangfankeji.com

[R27] 算术展开
来源：http://yqe.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://nim.fktsv.cn

[R28] 浮点运算
来源：http://wso.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://ltw.jinqigfzy.top

[R29] 定义函数
来源：http://frx.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xic.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://yif.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://xsu.cqqwz.cn

[R31] 局部变量
来源：http://vui.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://iax.ppjwa.cn

[R32] 参数个数校验
来源：http://lot.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mvp.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://hqv.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jop.hongshengwenyu.top

[R34] 退出时清理
来源：http://lhy.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://cpy.hesvh.cn

[R35] 后台执行并等待
来源：http://uwo.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ssw.zdbjq.cn

[R36] 并发执行多个任务
来源：http://mwr.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dbg.shzxlz.cn

[R37] 把输出赋给变量
来源：http://xpg.zdqjudy.top

files=$(ls -1)
来源：http://xwy.quarkkingdee.top

[R38] 管道串联
来源：http://qrt.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://mlk.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://hny.zdbjq.cn

cmd > out.log 2>&1
来源：http://bqy.yanxiufei.cn

[R40] 追加写日志
来源：http://gfw.hongshengwenyu.top

echo "log" >> out.log
来源：http://txe.yvedp.cn

[R41] 丢弃输出
来源：http://ews.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://ypv.zhongyouzk.top

[R42] 输入重定向
来源：http://jrc.gogol.net.cn

wc -l < a.txt
来源：http://cql.9152youxi.cn

[R43] 按名字查找文件
来源：http://bnm.gogol.net.cn

find . -name "*.log" -type f
来源：http://mmb.zhengqikj.top

[R44] 按修改时间查找
来源：http://xku.guannengcc.top

find . -mtime -7 -type f
来源：http://kah.mhx1999.top

[R45] 批量删除
来源：http://pfy.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://fer.xuanzx.com

[R46] 递归替换文件内容
来源：http://grk.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bwe.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://opp.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://hwb.cdnleiting.top

[R48] awk 取指定列
来源：http://num.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://smb.yonumen.top

[R49] awk 带条件
来源：http://amj.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ucu.jinqigfzy.top

[R50] awk 求和
来源：http://bqj.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zdh.yonumen.top

[R51] 排序去重取前几
来源：http://lzb.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yrb.fehbvm.com

[R52] 统计行数
来源：http://zax.iojbl.cn

wc -l a.txt
来源：http://wdd.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://iyp.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wec.zhongyouzk.top

[R54] 比较两个文件
来源：http://ixo.pengpengdd.cyou

diff a.txt b.txt
来源：http://shz.ppjwa.cn

[R55] 压缩与解压
来源：http://uih.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://swx.cucudq.cn

[R56] 远程拷贝
来源：http://ogi.meibo888.top

scp file user@host:/path/
来源：http://axi.dashuyun.cn

[R57] 远程执行命令
来源：http://dle.gotoacloud.top

ssh user@host 'uptime'
来源：http://hew.fanxiaobao.xyz

[R58] 下载文件
来源：http://hfj.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ziy.hywenlv.cn

[R59] 发 POST JSON
来源：http://rgo.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://egr.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://gff.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zxs.vqdsnc.cn

[R61] 磁盘占用
来源：http://zax.nanxinkj.top

df -h;  du -sh *
来源：http://wqg.dianchejie.cn

[R62] 找最占空间的文件
来源：http://kay.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://nlc.gotoacloud.top

[R63] 内存与进程
来源：http://ouv.cashguo.top

free -h;  ps aux | grep nginx
来源：http://otm.9152youxi.cn

[R64] 结束进程
来源：http://rvh.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://kqw.jiagoushi.top

[R65] 查看端口占用
来源：http://uvd.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rhk.nanxinkj.top

[R66] 定时任务
来源：http://onb.sufxvd.cn

crontab -e;  crontab -l
来源：http://rkb.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://ugu.xziqi.cn

openssl rand -hex 16
来源：http://rsd.daria6918.cn

[R68] 计算文件校验值
来源：http://pqr.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://sux.shuidangran.top

[R69] 生成随机密码
来源：http://cam.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://osh.316326.xyz

[R70] 时间戳与互转
来源：http://rmy.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://qgr.yueranfly.top

[R71] 日期格式化
来源：http://vtz.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mah.316326.xyz

[R72] 等待端口就绪
来源：http://wxe.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kpf.uphjek.com

[R73] 分割大日志
来源：http://vqs.hfpthk.cn

split -l 1000 big.log part_
来源：http://qqi.316326.xyz

[R74] 批量重命名
来源：http://zxz.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnr.sweek.top

[R75] 导出环境变量
来源：http://izm.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://zdn.hammf.cn

[R76] 使用临时文件
来源：http://yvf.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aam.birdmap.top

[R77] 读取用户输入
来源：http://ccu.zhijiandao.cn

read -rp "请输入: " ans
来源：http://zys.zhongyouzk.top

[R78] 交互式菜单
来源：http://lhk.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yuj.sxryk.cn

[R79] 解析命令行选项
来源：http://oxb.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eil.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://ifd.yj20258888.top

time ./run.sh
来源：http://yop.yanxiufei.cn

================================================================================
来源：http://itg.sjlbkw.cn

S. C / C++ 专题
来源：http://zhm.hongshengwenyu.top

================================================================================
来源：http://lkf.xuanzx.com

[S01] C：Hello World
来源：http://arh.haohaochexian.top

#include <stdio.h>
来源：http://vwp.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vsh.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://uep.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://pxu.quarkkingdee.top

[S03] C：读入整数
来源：http://cvz.zdbjq.cn

int x; scanf("%d", &x);
来源：http://yol.chenlongwang.top

[S04] C：字符串复制
来源：http://oqn.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qmf.chenlongwang.top

[S05] C：字符串长度
来源：http://jjp.jlsjyb.cn

strlen(s)
来源：http://adl.ctjpmb.com

[S06] C：字符串比较
来源：http://sck.birdmap.top

strcmp(a, b) == 0
来源：http://ffg.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://dec.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ccj.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://fiu.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://guf.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://jhr.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qsx.tian-w.cn

[S10] C：指针与解引用
来源：http://fnf.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://zbh.jlsjyb.cn

[S11] C：逐行读文件
来源：http://mth.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://crr.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nav.birdmap.top

fclose(f);
来源：http://kic.chenzaomai.com

[S12] C：写文件
来源：http://cbx.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dyx.yuxming.cn

[S13] C：宏定义
来源：http://ywe.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hwi.xuanzx.com

[S14] C：枚举
来源：http://oco.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://jhm.aizwys.cn

[S15] C：类型转换
来源：http://wcl.fanxiaobao.xyz

(double) a / b
来源：http://eps.gzhubu.top

[S16] C：位操作置位
来源：http://ugv.bjfxy.top

x |= (1 << 3);
来源：http://qxv.bbcook.cn

[S17] C：安全拼接字符串
来源：http://bvm.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iud.fengsongda.top

[S18] C：命令行参数
来源：http://vbi.xylfe.cn

int main(int argc, char **argv)
来源：http://lrs.zhiwuduotai.top

[S19] C：快速排序
来源：http://xgd.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bhj.yvedp.cn

[S20] C：二分查找
来源：http://eut.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ugx.cdnleiting.top

[S21] C：字符类别判断
来源：http://eei.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://egb.sysykeji.top

[S22] C：字符串转数字
来源：http://uyd.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nwp.guowangkeji.top

[S23] C：随机数
来源：http://qzn.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bcl.bbcook.cn

[S24] C：获取本地时间
来源：http://nks.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pwh.hfpthk.cn

[S25] C：内存拷贝
来源：http://unk.hfpthk.cn

memcpy(dst, src, n);
来源：http://yfc.jinqigfzy.top

[S26] C：内存清零
来源：http://tij.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://pfm.smart0.xyz

[S27] C：定义常量
来源：http://lww.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://blq.0kj1m.cn

[S28] C：静态变量
来源：http://qds.bbcook.cn

static int counter = 0;
来源：http://rnj.gogol.net.cn

[S29] C：变参函数
来源：http://ufm.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hvt.cucudq.cn

[S30] C：头文件保护
来源：http://ypy.yanxiufei.cn

#ifndef X_H
来源：http://jer.yangfankeji.com

#define X_H
来源：http://vlc.jinqigufen.top

#endif
来源：http://ihn.zhijiandao.cn

[S31] C++：Hello World
来源：http://qyb.jinghuilouyu.cn

#include <iostream>
来源：http://pyc.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://qjf.ydzc1.top

[S32] C++：字符串
来源：http://snv.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://gny.vehdjk.com

[S33] C++：vector 增删
来源：http://txe.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://owk.ydzc1.top

[S34] C++：遍历 vector
来源：http://tju.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://eyr.xuetiantiany.cn

[S35] C++：map
来源：http://dih.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yen.ybcxt.top

[S36] C++：unordered_map
来源：http://exz.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://owd.iojbl.cn

[S37] C++：set
来源：http://pow.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mlo.ydzc1.top

[S38] C++：排序
来源：http://xug.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://klm.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://ftu.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vpb.hnxiangtu.top

[S40] C++：查找元素
来源：http://mgv.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oeu.yj202588.top

[S41] C++：类与构造函数
来源：http://hux.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hxs.guannengcc.top

[S42] C++：继承与虚函数
来源：http://lha.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://wwl.wangdashe.top

[S43] C++：智能指针
来源：http://puj.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://zpp.sjlbkw.cn

[S44] C++：引用传参
来源：http://ajf.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://vpj.chenjidiqi.icu

[S45] C++：lambda
来源：http://rzx.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://wub.kuanghao11.cn

[S46] C++：函数模板
来源：http://sva.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qzp.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://mkw.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hot.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://xzi.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://zrh.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://knm.gzhubu.top

[S49] C++：写文件
来源：http://buf.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cgl.redwolf501.top

[S50] C++：格式化数字
来源：http://cnl.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hmj.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://aez.fzhhl.top

static_cast<double>(a) / b
来源：http://kzf.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://oph.tianlin.xyz


<!-- 参考信息 -->