代发 wailian999

[Q78] 当前时间
来源：http://xlk.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ljc.cqqwz.cn

[Q79] 字符串拼接
来源：http://wsc.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ilw.xuanzx.com

[Q80] 字符串截取
来源：http://kml.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://saj.jqgfzy.top

[Q81] 字符串替换
来源：http://maj.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zmz.pycfn.com

[Q82] 字符长度与字节长度
来源：http://exg.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ude.sxryk.cn

[Q83] 大小写转换
来源：http://xcx.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pri.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://hdv.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://day.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://tle.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gqb.meibo888.top

[Q86] 读取 JSON 字段
来源：http://fca.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ufv.fktsv.cn

[Q87] JSON 字段做条件
来源：http://poy.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wkj.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://lus.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nqz.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rdp.snrcjt.cn

[Q89] 判断表是否存在
来源：http://hoh.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xup.uphjek.com

[Q90] 生成序号列
来源：http://eha.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://syv.birdmap.top

================================================================================
来源：http://yuo.0kj1m.cn

R. Bash 专题
来源：http://euo.hysaishi.cn

================================================================================
来源：http://ygv.dashuyun.cn

[R01] shebang 与严格模式
来源：http://plm.yongpay.top

#!/usr/bin/env bash
来源：http://wjy.jinqigfzy.top

set -euo pipefail
来源：http://brh.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://dlz.yongpay.top

name="Tom"; echo "$name"
来源：http://ibm.sweek.top

[R03] 只读变量
来源：http://byz.fktsv.cn

readonly PI=3.14
来源：http://vkc.iojbl.cn

[R04] 位置参数
来源：http://dsh.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edk.birdmap.top

[R05] 参数默认值
来源：http://bdt.yj202588.top

name="${1:-default}"
来源：http://lfd.hysaishi.cn

[R06] 判断命令是否存在
来源：http://wmr.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://igv.yonumen.top

[R07] if 判断文件
来源：http://rpo.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://brf.epnwcf.com

[R08] 数值比较
来源：http://qzt.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iqh.shzxlz.cn

[R09] 字符串比较
来源：http://let.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lxz.yuanzhike.top

[R10] 正则匹配
来源：http://zel.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://adm.mhx1999.top

[R11] case 多分支
来源：http://zrb.wangdashe.top

case "$1" in
来源：http://jne.yangfankeji.com

start) echo "启动" ;;
来源：http://rfl.xuanzx.com

stop)  echo "停止" ;;
来源：http://bzr.yongpay.top

*)     echo "未知命令" ;;
来源：http://kgm.vqdsnc.cn

esac
来源：http://rex.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://asl.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://fbm.jianghu66.top

[R13] for 计数循环
来源：http://cct.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://lqj.ydjk.org.cn

[R14] C 风格 for
来源：http://lxr.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gif.tianlin.xyz

[R15] while 逐行读文件
来源：http://wlu.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qud.cqqwz.cn

[R16] until 等待条件
来源：http://gpp.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwf.chenzaomai.com

[R17] 数组定义与取值
来源：http://hfk.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://kqh.shzxlz.cn

[R18] 遍历数组
来源：http://jud.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ogk.feifeiyinyue.top

[R19] 数组长度
来源：http://nzb.yj20258888.top

echo "${#arr[@]}"
来源：http://idk.gzhubu.top

[R20] 关联数组（字典）
来源：http://xlz.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vsf.pengpengdd.cyou

[R21] 字符串长度
来源：http://ims.daxiang520.top

echo "${#s}"
来源：http://olc.zhixingplan.top

[R22] 截取子串
来源：http://xmt.cashguo.top

echo "${s:0:5}"
来源：http://axt.hnxiangtu.top

[R23] 字符串替换
来源：http://nya.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aza.birdmap.top

[R24] 大小写转换
来源：http://wvc.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://rqs.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://sxi.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ubs.fzhhl.top

[R26] 命令替换
来源：http://fff.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://sjn.yueranfly.top

[R27] 算术展开
来源：http://vma.cucudq.cn

echo $((1 + 2 * 3))
来源：http://jom.cucudq.cn

[R28] 浮点运算
来源：http://tuy.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://aab.gogol.net.cn

[R29] 定义函数
来源：http://blg.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bfi.chenzaomai.com

[R30] 函数返回状态码
来源：http://dra.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://eyv.zhixingplan.top

[R31] 局部变量
来源：http://hks.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://uhc.jinqigufen.top

[R32] 参数个数校验
来源：http://byl.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mss.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://dfl.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ybt.cucudq.cn

[R34] 退出时清理
来源：http://sag.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://jti.hnxiangtu.top

[R35] 后台执行并等待
来源：http://zes.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mbs.ybcxt.top

[R36] 并发执行多个任务
来源：http://lij.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kqx.smart0.xyz

[R37] 把输出赋给变量
来源：http://pjg.xuanzx.com

files=$(ls -1)
来源：http://hfl.chenjidiqi.icu

[R38] 管道串联
来源：http://aoj.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://agb.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://bjj.hammf.cn

cmd > out.log 2>&1
来源：http://jvh.iojbl.cn

[R40] 追加写日志
来源：http://xeo.vqdsnc.cn

echo "log" >> out.log
来源：http://rhd.tian-w.cn

[R41] 丢弃输出
来源：http://bpt.xuanzx.com

cmd >/dev/null 2>&1
来源：http://yve.yj202588.top

[R42] 输入重定向
来源：http://jmj.shanyushiyangkeji.top

wc -l < a.txt
来源：http://phn.cucudq.cn

[R43] 按名字查找文件
来源：http://tdd.pycfn.com

find . -name "*.log" -type f
来源：http://uzv.ivvv.top

[R44] 按修改时间查找
来源：http://crd.yfazqb.com

find . -mtime -7 -type f
来源：http://mgq.cheryme.top

[R45] 批量删除
来源：http://yaz.yonumen.top

find . -name "*.tmp" -delete
来源：http://fjz.zhixingplan.top

[R46] 递归替换文件内容
来源：http://syl.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://znc.hammf.cn

[R47] sed 单行替换
来源：http://uny.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://hei.shuidangran.top

[R48] awk 取指定列
来源：http://izi.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://lbe.uphjek.com

[R49] awk 带条件
来源：http://feg.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ltx.jlsjyb.cn

[R50] awk 求和
来源：http://nqh.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://gux.iojbl.cn

[R51] 排序去重取前几
来源：http://scl.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dtj.iojbl.cn

[R52] 统计行数
来源：http://knm.xuetiantiany.cn

wc -l a.txt
来源：http://wof.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://ifa.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jdk.kuanghao11.cn

[R54] 比较两个文件
来源：http://mpv.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://xyk.aibaodan.cn

[R55] 压缩与解压
来源：http://qta.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ihv.xziqi.cn

[R56] 远程拷贝
来源：http://dpb.bbcook.cn

scp file user@host:/path/
来源：http://eod.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://hdv.hysaishi.cn

ssh user@host 'uptime'
来源：http://dpe.jianghu66.top

[R58] 下载文件
来源：http://zjx.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vkd.birdmap.top

[R59] 发 POST JSON
来源：http://vko.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bbo.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://wtt.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aab.sjlbkw.cn

[R61] 磁盘占用
来源：http://yry.jinghuilouyu.cn

df -h;  du -sh *
来源：http://flc.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://gyg.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://unz.shangyingyoupin.top

[R63] 内存与进程
来源：http://oii.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://znk.tanke756.top

[R64] 结束进程
来源：http://ixb.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://czx.wangshuangyany.cn

[R65] 查看端口占用
来源：http://ros.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://exn.dashuyun.cn

[R66] 定时任务
来源：http://non.jiagoushi.top

crontab -e;  crontab -l
来源：http://wqk.shuidangran.top

[R67] 生成随机十六进制串
来源：http://wyh.jqgfzy.top

openssl rand -hex 16
来源：http://tre.yongpay.top

[R68] 计算文件校验值
来源：http://rss.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://ozl.gaohongyu789.top

[R69] 生成随机密码
来源：http://dyz.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://orb.zdbjq.cn

[R70] 时间戳与互转
来源：http://hbf.wangdashe.top

date +%s;  date -d @1700000000
来源：http://wuv.yj202588.top

[R71] 日期格式化
来源：http://jjs.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zxe.guannengcc.top

[R72] 等待端口就绪
来源：http://ahh.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aqn.uphjek.com

[R73] 分割大日志
来源：http://stt.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://cxj.nanxuanxn.top

[R74] 批量重命名
来源：http://rke.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://slg.hcnkem.com

[R75] 导出环境变量
来源：http://gcn.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://vxc.gaohongyu789.top

[R76] 使用临时文件
来源：http://ngl.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pew.hywenlv.cn

[R77] 读取用户输入
来源：http://ujp.yvedp.cn

read -rp "请输入: " ans
来源：http://ejp.pengpengdd.cyou

[R78] 交互式菜单
来源：http://dyh.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wdu.zhijiandao.cn

[R79] 解析命令行选项
来源：http://fpb.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qbh.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://kaf.shanyushiyangtech.top

time ./run.sh
来源：http://wro.jinqigfzy.top

================================================================================
来源：http://brl.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://ljs.tian-w.cn

================================================================================
来源：http://irc.xylfe.cn

[S01] C：Hello World
来源：http://qec.hammf.cn

#include <stdio.h>
来源：http://bzs.pycfn.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jkg.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://fhn.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://brq.ppjwa.cn

[S03] C：读入整数
来源：http://bgc.sweek.top

int x; scanf("%d", &x);
来源：http://uub.redwolf501.top

[S04] C：字符串复制
来源：http://uff.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ksj.bbcook.cn

[S05] C：字符串长度
来源：http://ksf.yonumen.top

strlen(s)
来源：http://aue.tanke756.top

[S06] C：字符串比较
来源：http://zut.yfazqb.com

strcmp(a, b) == 0
来源：http://wpz.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://dby.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vki.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://zws.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ilf.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://nhp.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ptv.sysykeji.top

[S10] C：指针与解引用
来源：http://mof.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://jtx.nwbrower.top

[S11] C：逐行读文件
来源：http://ngb.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://csi.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jkn.yonumen.top

fclose(f);
来源：http://npy.xuanzx.com

[S12] C：写文件
来源：http://ggn.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uxw.zdqjudy.top

[S13] C：宏定义
来源：http://vek.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oiq.daxiang520.top

[S14] C：枚举
来源：http://gex.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://zsx.yuxming.cn

[S15] C：类型转换
来源：http://hbo.yonumen.top

(double) a / b
来源：http://mub.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://beg.guowangkeji.top

x |= (1 << 3);
来源：http://bns.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://cmm.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uyy.guannengcc.top

[S18] C：命令行参数
来源：http://inb.jinqigfzy.top

int main(int argc, char **argv)
来源：http://rjy.chenzaomai.com

[S19] C：快速排序
来源：http://txt.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://hoc.ctjpmb.com

[S20] C：二分查找
来源：http://tbi.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jzf.andypj.xyz

[S21] C：字符类别判断
来源：http://jbz.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tqd.snrcjt.cn

[S22] C：字符串转数字
来源：http://wuv.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://wzd.kuanghao11.cn

[S23] C：随机数
来源：http://pev.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eol.nanxinkj.top

[S24] C：获取本地时间
来源：http://xfm.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lbf.pycfn.com

[S25] C：内存拷贝
来源：http://nuk.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://nhb.gogol.net.cn

[S26] C：内存清零
来源：http://tlw.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://skw.shzxlz.cn

[S27] C：定义常量
来源：http://spa.sjlbkw.cn

const double PI = 3.14159;
来源：http://eue.iojbl.cn

[S28] C：静态变量
来源：http://mcm.dianchejie.cn

static int counter = 0;
来源：http://iqq.zhiwuduotai.top

[S29] C：变参函数
来源：http://klc.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ssq.jinqigufen.top

[S30] C：头文件保护
来源：http://egf.zhixingplan.top

#ifndef X_H
来源：http://dhb.vehdjk.com

#define X_H
来源：http://nzr.bjfxy.top

#endif
来源：http://sxi.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://lqj.hywenlv.cn

#include <iostream>
来源：http://thf.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://edk.fanxiaobao.xyz

[S32] C++：字符串
来源：http://rgl.hammf.cn

std::string s = "hi";  s += "!";
来源：http://rif.jianghu66.top

[S33] C++：vector 增删
来源：http://kxf.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tak.yuxming.cn

[S34] C++：遍历 vector
来源：http://ynd.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://vsn.havefunace.top

[S35] C++：map
来源：http://hsk.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhk.c1oappe.top

[S36] C++：unordered_map
来源：http://bay.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nrm.zhaomingkeji.xyz

[S37] C++：set
来源：http://mbf.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lpo.cucudq.cn

[S38] C++：排序
来源：http://xgt.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://jpg.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://jfk.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ctb.zdqjudy.top

[S40] C++：查找元素
来源：http://ogq.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://etu.ydzc1.top

[S41] C++：类与构造函数
来源：http://wpp.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xyi.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://sxn.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://swm.yonumen.top

[S43] C++：智能指针
来源：http://axn.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://mka.ybcxt.top

[S44] C++：引用传参
来源：http://bob.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://gsr.ctjpmb.com

[S45] C++：lambda
来源：http://lxm.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://acb.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://zat.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dbx.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://duh.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zcn.shzxlz.cn

[S48] C++：逐行读文件
来源：http://pdx.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cfz.ctjpmb.com


<!-- 参考信息 -->