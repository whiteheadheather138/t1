代发 wailian999

[Q78] 当前时间
来源：http://kog.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jry.chenlongwang.top

[Q79] 字符串拼接
来源：http://ngh.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oor.uphjek.com

[Q80] 字符串截取
来源：http://sfz.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hei.hysaishi.cn

[Q81] 字符串替换
来源：http://jvv.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ndf.yonumen.top

[Q82] 字符长度与字节长度
来源：http://lwe.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://upe.yvedp.cn

[Q83] 大小写转换
来源：http://klb.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pwm.epnwcf.com

[Q84] 去除首尾空格
来源：http://ipj.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://hoy.zhoulong.xyz

[Q85] 数值取整
来源：http://dtm.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gav.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://psi.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ncu.daxiang520.top

[Q87] JSON 字段做条件
来源：http://rng.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iyg.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://gwu.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pyq.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jzk.mhx1999.top

[Q89] 判断表是否存在
来源：http://vba.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jpf.havefunace.top

[Q90] 生成序号列
来源：http://sre.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vgg.iojbl.cn

================================================================================
来源：http://yzr.kuanghao11.cn

R. Bash 专题
来源：http://gvh.shuidangran.top

================================================================================
来源：http://enh.hywenlv.cn

[R01] shebang 与严格模式
来源：http://jkk.zhijiandao.cn

#!/usr/bin/env bash
来源：http://thj.kuanghao11.cn

set -euo pipefail
来源：http://jns.uphjek.com

[R02] 变量赋值与使用
来源：http://ofy.dianchejie.cn

name="Tom"; echo "$name"
来源：http://ciq.zhongyouzk.top

[R03] 只读变量
来源：http://xco.yj20258888.top

readonly PI=3.14
来源：http://cnd.316326.xyz

[R04] 位置参数
来源：http://mhe.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fqw.hysaishi.cn

[R05] 参数默认值
来源：http://wms.dianchejie.cn

name="${1:-default}"
来源：http://cid.aibaodan.cn

[R06] 判断命令是否存在
来源：http://jkb.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yzs.yfazqb.com

[R07] if 判断文件
来源：http://lty.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ark.kuanghao11.cn

[R08] 数值比较
来源：http://yhm.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bcz.zhongyouzk.top

[R09] 字符串比较
来源：http://bgl.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jkz.fengsongda.top

[R10] 正则匹配
来源：http://qar.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lsc.52xcode.cn

[R11] case 多分支
来源：http://lyl.fzhhl.top

case "$1" in
来源：http://pcy.fehbvm.com

start) echo "启动" ;;
来源：http://xtp.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://svg.uphjek.com

*)     echo "未知命令" ;;
来源：http://klv.zhengqikj.top

esac
来源：http://oip.gotoacloud.top

[R12] for 遍历文件
来源：http://kqj.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://dwd.shuidangran.top

[R13] for 计数循环
来源：http://dfy.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://esk.ivvv.top

[R14] C 风格 for
来源：http://fqy.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfm.dashuyun.cn

[R15] while 逐行读文件
来源：http://vjj.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vcx.hysaishi.cn

[R16] until 等待条件
来源：http://hhc.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sbh.hesvh.cn

[R17] 数组定义与取值
来源：http://nml.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lbz.gaohongyu789.top

[R18] 遍历数组
来源：http://vhh.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdx.hywenlv.cn

[R19] 数组长度
来源：http://qhx.zycfv.cn

echo "${#arr[@]}"
来源：http://faj.dianchejie.cn

[R20] 关联数组（字典）
来源：http://xpd.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://njr.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://wfv.havefunace.top

echo "${#s}"
来源：http://lht.shanyushiyangkeji.top

[R22] 截取子串
来源：http://fys.ydjk.org.cn

echo "${s:0:5}"
来源：http://pfy.jinqigfzy.top

[R23] 字符串替换
来源：http://nrf.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://owj.ydzc1.top

[R24] 大小写转换
来源：http://zbq.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://kxe.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://sgj.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://msc.xinyue.icu

[R26] 命令替换
来源：http://kca.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://bkj.birdmap.top

[R27] 算术展开
来源：http://gny.redwolf501.top

echo $((1 + 2 * 3))
来源：http://pxv.jinqigufen.top

[R28] 浮点运算
来源：http://cis.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://ntf.hammf.cn

[R29] 定义函数
来源：http://dfw.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yya.hcnkem.com

[R30] 函数返回状态码
来源：http://wcl.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://zbn.ydjk.org.cn

[R31] 局部变量
来源：http://wht.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://zly.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://xft.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qzu.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://jpi.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fdx.xziqi.cn

[R34] 退出时清理
来源：http://lhe.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://mct.hcnkem.com

[R35] 后台执行并等待
来源：http://wnv.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xqg.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://vuv.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://krx.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://neq.fehbvm.com

files=$(ls -1)
来源：http://poe.cucudq.cn

[R38] 管道串联
来源：http://cjm.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://xrz.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://lfn.yuanzhike.top

cmd > out.log 2>&1
来源：http://arw.chenjidiqi.icu

[R40] 追加写日志
来源：http://anj.xylfe.cn

echo "log" >> out.log
来源：http://uax.yfazqb.com

[R41] 丢弃输出
来源：http://xoy.sweek.top

cmd >/dev/null 2>&1
来源：http://qae.316326.xyz

[R42] 输入重定向
来源：http://dor.haohaochexian.top

wc -l < a.txt
来源：http://lyt.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://zuv.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://htt.sufxvd.cn

[R44] 按修改时间查找
来源：http://rqo.yfazqb.com

find . -mtime -7 -type f
来源：http://vou.svipenyu.cn

[R45] 批量删除
来源：http://yrj.xuanzx.com

find . -name "*.tmp" -delete
来源：http://vzo.snrcjt.cn

[R46] 递归替换文件内容
来源：http://blw.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gze.xziqi.cn

[R47] sed 单行替换
来源：http://gtz.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mlh.vqdsnc.cn

[R48] awk 取指定列
来源：http://mao.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://gdn.tianlin.xyz

[R49] awk 带条件
来源：http://rcp.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tke.guowangkeji.top

[R50] awk 求和
来源：http://yme.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://lbr.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://tyk.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tda.svipenyu.cn

[R52] 统计行数
来源：http://gav.hammf.cn

wc -l a.txt
来源：http://oyl.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://yng.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rll.ehwqpu.com

[R54] 比较两个文件
来源：http://izf.haohaochexian.top

diff a.txt b.txt
来源：http://ens.cqqwz.cn

[R55] 压缩与解压
来源：http://sih.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulg.c1oappe.top

[R56] 远程拷贝
来源：http://xhr.yj202588.top

scp file user@host:/path/
来源：http://idx.zhongyouzk.top

[R57] 远程执行命令
来源：http://vom.ydjk.org.cn

ssh user@host 'uptime'
来源：http://djx.aizwys.cn

[R58] 下载文件
来源：http://uhe.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gek.jqgfzy.top

[R59] 发 POST JSON
来源：http://hqw.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eou.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://zxq.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fph.sweek.top

[R61] 磁盘占用
来源：http://arx.aibaodan.cn

df -h;  du -sh *
来源：http://uvo.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://dcp.cheryme.top

du -ah . | sort -rh | head -10
来源：http://xdy.ctjpmb.com

[R63] 内存与进程
来源：http://tbf.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://qhe.shanyushiyangtech.top

[R64] 结束进程
来源：http://rmg.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://apm.zdqjudy.top

[R65] 查看端口占用
来源：http://xzo.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eng.bjfxy.top

[R66] 定时任务
来源：http://svg.vqdsnc.cn

crontab -e;  crontab -l
来源：http://kpe.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://bvg.ybcxt.top

openssl rand -hex 16
来源：http://djj.yj20258888.top

[R68] 计算文件校验值
来源：http://hhx.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://xfn.aizwys.cn

[R69] 生成随机密码
来源：http://puf.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://dud.ppjwa.cn

[R70] 时间戳与互转
来源：http://wgx.316326.xyz

date +%s;  date -d @1700000000
来源：http://lxq.daria6918.cn

[R71] 日期格式化
来源：http://alv.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qjh.ppjwa.cn

[R72] 等待端口就绪
来源：http://woa.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jhl.pengpengdd.cyou

[R73] 分割大日志
来源：http://lny.shuidangran.top

split -l 1000 big.log part_
来源：http://yvg.hysaishi.cn

[R74] 批量重命名
来源：http://jxc.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zfw.hcnkem.com

[R75] 导出环境变量
来源：http://ywj.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://azx.52xcode.cn

[R76] 使用临时文件
来源：http://uhh.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vck.nwbrower.top

[R77] 读取用户输入
来源：http://ivk.cqqwz.cn

read -rp "请输入: " ans
来源：http://ulz.zhixingplan.top

[R78] 交互式菜单
来源：http://oju.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://dva.cheryme.top

[R79] 解析命令行选项
来源：http://byv.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzu.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://khx.svipenyu.cn

time ./run.sh
来源：http://nek.quarkkingdee.top

================================================================================
来源：http://enf.zdqjudy.top

S. C / C++ 专题
来源：http://gzb.jiagoushi.top

================================================================================
来源：http://mbd.vqdsnc.cn

[S01] C：Hello World
来源：http://kgp.ppjwa.cn

#include <stdio.h>
来源：http://gtp.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ecq.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://wqr.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://vai.fktsv.cn

[S03] C：读入整数
来源：http://fhi.yueranfly.top

int x; scanf("%d", &x);
来源：http://fuv.fehbvm.com

[S04] C：字符串复制
来源：http://qku.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://jyu.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://hsn.dianchejie.cn

strlen(s)
来源：http://gck.wangshuangyany.cn

[S06] C：字符串比较
来源：http://rrd.snrcjt.cn

strcmp(a, b) == 0
来源：http://zta.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://ijk.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fim.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://gei.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bhy.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://rnf.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bik.ybcxt.top

[S10] C：指针与解引用
来源：http://vhc.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://jdx.wangdashe.top

[S11] C：逐行读文件
来源：http://hzr.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://pxp.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nif.ctjpmb.com

fclose(f);
来源：http://ezp.tanke756.top

[S12] C：写文件
来源：http://grm.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sdm.yueranfly.top

[S13] C：宏定义
来源：http://sgf.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://asv.hammf.cn

[S14] C：枚举
来源：http://vim.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://xoq.tian-w.cn

[S15] C：类型转换
来源：http://wjv.c1oappe.top

(double) a / b
来源：http://gfq.c1oappe.top

[S16] C：位操作置位
来源：http://yoz.jinghuilouyu.cn

x |= (1 << 3);
来源：http://nyr.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://noi.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pst.ydzc1.top

[S18] C：命令行参数
来源：http://iug.guannengcc.top

int main(int argc, char **argv)
来源：http://mqv.hnxiangtu.top

[S19] C：快速排序
来源：http://kmp.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gyg.feifeiyinyue.top

[S20] C：二分查找
来源：http://cwy.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mas.c1oappe.top

[S21] C：字符类别判断
来源：http://rtb.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zfh.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://eoe.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fow.316326.xyz

[S23] C：随机数
来源：http://wnb.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://roh.nwbrower.top

[S24] C：获取本地时间
来源：http://dvz.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://buq.jinqigufen.top

[S25] C：内存拷贝
来源：http://zbe.meibo888.top

memcpy(dst, src, n);
来源：http://jmm.yj20258888.top

[S26] C：内存清零
来源：http://hko.yuxming.cn

memset(a, 0, sizeof a);
来源：http://lbr.xinyue.icu

[S27] C：定义常量
来源：http://nzp.zhengqikj.top

const double PI = 3.14159;
来源：http://thx.xziqi.cn

[S28] C：静态变量
来源：http://wht.hnxiangtu.top

static int counter = 0;
来源：http://xuz.52xcode.cn

[S29] C：变参函数
来源：http://muy.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ajt.yj20258888.top

[S30] C：头文件保护
来源：http://wgy.iojbl.cn

#ifndef X_H
来源：http://aph.xinyue.icu

#define X_H
来源：http://kuy.yj20258.top

#endif
来源：http://vof.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://nka.ppjwa.cn

#include <iostream>
来源：http://exs.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://dfr.wangdashe.top

[S32] C++：字符串
来源：http://lan.sweek.top

std::string s = "hi";  s += "!";
来源：http://jrz.yuanzhike.top

[S33] C++：vector 增删
来源：http://swt.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oic.andypj.xyz

[S34] C++：遍历 vector
来源：http://rne.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://opu.ydjk.org.cn

[S35] C++：map
来源：http://agg.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://euf.yfazqb.com

[S36] C++：unordered_map
来源：http://wuf.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tfw.kuanghao11.cn

[S37] C++：set
来源：http://zgx.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ozv.chenzaomai.com

[S38] C++：排序
来源：http://jxw.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://bzx.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://xrb.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rno.shuidangran.top

[S40] C++：查找元素
来源：http://otb.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fab.wangdashe.top

[S41] C++：类与构造函数
来源：http://wyv.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ovh.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://lwe.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://krv.redwolf501.top

[S43] C++：智能指针
来源：http://quu.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://siw.feifeiyinyue.top

[S44] C++：引用传参
来源：http://pth.gzhubu.top

void inc(int &x) { ++x; }
来源：http://iwi.tianlin.xyz

[S45] C++：lambda
来源：http://zht.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://sdr.9152youxi.cn

[S46] C++：函数模板
来源：http://vqv.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zcb.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://iwz.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ueb.ctjpmb.com

[S48] C++：逐行读文件
来源：http://dne.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://etr.meibo888.top


<!-- 参考信息 -->