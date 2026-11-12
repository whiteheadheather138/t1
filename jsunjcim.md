代发 wailian999

[Q78] 当前时间
来源：http://tmq.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vzf.haohaochexian.top

[Q79] 字符串拼接
来源：http://woi.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://afa.zhongyouzk.top

[Q80] 字符串截取
来源：http://ykt.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yly.xuanzx.com

[Q81] 字符串替换
来源：http://gey.yueranfly.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xzi.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://mly.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nvl.yonumen.top

[Q83] 大小写转换
来源：http://swu.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lpm.meibo888.top

[Q84] 去除首尾空格
来源：http://uib.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://tho.meibo888.top

[Q85] 数值取整
来源：http://uze.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ozp.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://btp.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ctv.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://prl.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zuf.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://eee.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mxi.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rnp.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://wfj.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xox.0kj1m.cn

[Q90] 生成序号列
来源：http://bii.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://noi.ehwqpu.com

================================================================================
来源：http://ogw.zhaomingkeji.xyz

R. Bash 专题
来源：http://lwe.zhoulong.xyz

================================================================================
来源：http://coa.ivvv.top

[R01] shebang 与严格模式
来源：http://ycj.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://hhm.yj202588.top

set -euo pipefail
来源：http://svv.ybcxt.top

[R02] 变量赋值与使用
来源：http://ubw.ppjwa.cn

name="Tom"; echo "$name"
来源：http://wvh.gzhubu.top

[R03] 只读变量
来源：http://kzb.jianghu66.top

readonly PI=3.14
来源：http://uxn.yj20258.top

[R04] 位置参数
来源：http://rbz.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pak.0kj1m.cn

[R05] 参数默认值
来源：http://vzx.pengpengdd.cyou

name="${1:-default}"
来源：http://asb.9152youxi.cn

[R06] 判断命令是否存在
来源：http://ejt.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wiz.hfpthk.cn

[R07] if 判断文件
来源：http://pbo.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uub.shzxlz.cn

[R08] 数值比较
来源：http://omd.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dip.aizwys.cn

[R09] 字符串比较
来源：http://gkr.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rvs.shzxlz.cn

[R10] 正则匹配
来源：http://xyu.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hwu.zhaomingkeji.xyz

[R11] case 多分支
来源：http://dtq.hcnkem.com

case "$1" in
来源：http://atr.zhoulong.xyz

start) echo "启动" ;;
来源：http://mbr.xylfe.cn

stop)  echo "停止" ;;
来源：http://qam.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://spr.bbcook.cn

esac
来源：http://smw.zhiwuduotai.top

[R12] for 遍历文件
来源：http://quj.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://bsz.pengpengdd.cyou

[R13] for 计数循环
来源：http://wgs.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://okf.ivvv.top

[R14] C 风格 for
来源：http://wgy.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqg.tanke756.top

[R15] while 逐行读文件
来源：http://sup.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xlc.fengsongda.top

[R16] until 等待条件
来源：http://fqs.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bka.hywenlv.cn

[R17] 数组定义与取值
来源：http://xoy.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://qzf.daxiang520.top

[R18] 遍历数组
来源：http://xef.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://afg.tarul.cn

[R19] 数组长度
来源：http://dvh.yanxiufei.cn

echo "${#arr[@]}"
来源：http://jys.birdmap.top

[R20] 关联数组（字典）
来源：http://lfx.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://chj.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://rvk.xuanzx.com

echo "${#s}"
来源：http://udt.c1oappe.top

[R22] 截取子串
来源：http://abq.andypj.xyz

echo "${s:0:5}"
来源：http://hap.gogol.net.cn

[R23] 字符串替换
来源：http://phx.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mjb.chenlongwang.top

[R24] 大小写转换
来源：http://gvc.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://wpr.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://nvp.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gtl.hcnkem.com

[R26] 命令替换
来源：http://ktn.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://bul.shanyushiyangkeji.top

[R27] 算术展开
来源：http://pvm.yonumen.top

echo $((1 + 2 * 3))
来源：http://bbo.vehdjk.com

[R28] 浮点运算
来源：http://yjp.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://gnf.jinqigfzy.top

[R29] 定义函数
来源：http://nuy.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bob.yongpay.top

[R30] 函数返回状态码
来源：http://gox.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://onk.shanyushiyangtech.top

[R31] 局部变量
来源：http://ykt.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://ibp.chenzaomai.com

[R32] 参数个数校验
来源：http://fmn.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xrs.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://fuk.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ffq.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://jsg.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://bhu.kuanghao11.cn

[R35] 后台执行并等待
来源：http://dqi.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gau.hammf.cn

[R36] 并发执行多个任务
来源：http://wrx.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://agb.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://qsz.zycfv.cn

files=$(ls -1)
来源：http://tok.chenlongwang.top

[R38] 管道串联
来源：http://flr.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://koc.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://inp.ivvv.top

cmd > out.log 2>&1
来源：http://huz.hnxiangtu.top

[R40] 追加写日志
来源：http://dgy.tarul.cn

echo "log" >> out.log
来源：http://wec.tanke756.top

[R41] 丢弃输出
来源：http://lnn.redwolf501.top

cmd >/dev/null 2>&1
来源：http://dzm.ctjpmb.com

[R42] 输入重定向
来源：http://nop.tian-w.cn

wc -l < a.txt
来源：http://tsv.hysaishi.cn

[R43] 按名字查找文件
来源：http://yvj.yj202588.top

find . -name "*.log" -type f
来源：http://dmz.quarkkingdee.top

[R44] 按修改时间查找
来源：http://vvw.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://hxv.zhongyouzk.top

[R45] 批量删除
来源：http://pof.ydzc1.top

find . -name "*.tmp" -delete
来源：http://aka.jiagoushi.top

[R46] 递归替换文件内容
来源：http://wet.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://shq.jinqigfzy.top

[R47] sed 单行替换
来源：http://liq.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://vma.nanxinkj.top

[R48] awk 取指定列
来源：http://hgv.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://jhb.guowangkeji.top

[R49] awk 带条件
来源：http://iwu.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qac.shangyingyoupin.top

[R50] awk 求和
来源：http://lbt.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://vvu.gogol.net.cn

[R51] 排序去重取前几
来源：http://enu.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zwx.52xcode.cn

[R52] 统计行数
来源：http://fxf.316326.xyz

wc -l a.txt
来源：http://ysa.316326.xyz

[R53] 查看文件头与实时尾
来源：http://whl.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gcw.hnqzz.top

[R54] 比较两个文件
来源：http://doy.c1oappe.top

diff a.txt b.txt
来源：http://evh.chenjidiqi.icu

[R55] 压缩与解压
来源：http://pyc.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xxu.meibo888.top

[R56] 远程拷贝
来源：http://tqt.quarkkingdee.top

scp file user@host:/path/
来源：http://wuz.fktsv.cn

[R57] 远程执行命令
来源：http://ylz.meibo888.top

ssh user@host 'uptime'
来源：http://ecz.yongpay.top

[R58] 下载文件
来源：http://jxq.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cqf.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://dhc.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eyd.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://fpc.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iwh.ppjwa.cn

[R61] 磁盘占用
来源：http://itx.hesvh.cn

df -h;  du -sh *
来源：http://upo.ydzc1.top

[R62] 找最占空间的文件
来源：http://gwq.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://loj.yvedp.cn

[R63] 内存与进程
来源：http://one.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://ewh.ybcxt.top

[R64] 结束进程
来源：http://eok.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://ipi.yuanzhike.top

[R65] 查看端口占用
来源：http://vno.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpx.zdbjq.cn

[R66] 定时任务
来源：http://gea.dianchejie.cn

crontab -e;  crontab -l
来源：http://vvm.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://mdj.yuxming.cn

openssl rand -hex 16
来源：http://jth.52xcode.cn

[R68] 计算文件校验值
来源：http://wiv.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://bhe.yonumen.top

[R69] 生成随机密码
来源：http://jxc.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://lsu.fktsv.cn

[R70] 时间戳与互转
来源：http://qxd.yongpay.top

date +%s;  date -d @1700000000
来源：http://zun.hnxiangtu.top

[R71] 日期格式化
来源：http://qap.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kxf.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://lok.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://szo.52xcode.cn

[R73] 分割大日志
来源：http://acm.bjfxy.top

split -l 1000 big.log part_
来源：http://oee.jqgufenzy.top

[R74] 批量重命名
来源：http://fkh.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cus.zhiwuduotai.top

[R75] 导出环境变量
来源：http://zgi.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://dvr.chenjidiqi.icu

[R76] 使用临时文件
来源：http://rgb.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cam.yj20258.top

[R77] 读取用户输入
来源：http://jhz.hammf.cn

read -rp "请输入: " ans
来源：http://kum.c1oappe.top

[R78] 交互式菜单
来源：http://xfw.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://doc.vehdjk.com

[R79] 解析命令行选项
来源：http://dgg.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cft.ivvv.top

[R80] 查看脚本执行耗时
来源：http://aia.havefunace.top

time ./run.sh
来源：http://dup.smart0.xyz

================================================================================
来源：http://phq.bbcook.cn

S. C / C++ 专题
来源：http://vvv.ydjk.org.cn

================================================================================
来源：http://dvw.jianghu66.top

[S01] C：Hello World
来源：http://byx.shuidangran.top

#include <stdio.h>
来源：http://lxp.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://fqt.yuxming.cn

[S02] C：变量与格式化输出
来源：http://mqf.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://ppl.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://urh.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://qzv.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://foh.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://roh.epnwcf.com

[S05] C：字符串长度
来源：http://phy.birdmap.top

strlen(s)
来源：http://yrf.epnwcf.com

[S06] C：字符串比较
来源：http://xom.yueranfly.top

strcmp(a, b) == 0
来源：http://xeb.dianchejie.cn

[S07] C：数组遍历求和
来源：http://czw.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ksa.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://xyu.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hhi.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://pnq.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zys.jlsjyb.cn

[S10] C：指针与解引用
来源：http://vsc.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://amw.fzhhl.top

[S11] C：逐行读文件
来源：http://isx.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://uap.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://ybp.c1oappe.top

fclose(f);
来源：http://qua.cdnleiting.top

[S12] C：写文件
来源：http://qac.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pbi.feifeiyinyue.top

[S13] C：宏定义
来源：http://tqj.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://njr.yangfankeji.com

[S14] C：枚举
来源：http://abu.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://iih.zdbjq.cn

[S15] C：类型转换
来源：http://zsg.yuxming.cn

(double) a / b
来源：http://wye.zhongyouzk.top

[S16] C：位操作置位
来源：http://qrj.0kj1m.cn

x |= (1 << 3);
来源：http://ruz.fengsongda.top

[S17] C：安全拼接字符串
来源：http://brh.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tmn.zhiwuduotai.top

[S18] C：命令行参数
来源：http://hdy.guowangkeji.top

int main(int argc, char **argv)
来源：http://dro.ybcxt.top

[S19] C：快速排序
来源：http://qhe.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://nto.daria6918.cn

[S20] C：二分查找
来源：http://npd.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rat.yuxming.cn

[S21] C：字符类别判断
来源：http://zit.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pak.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://vly.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ixp.jinqigfzy.top

[S23] C：随机数
来源：http://emw.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://fdq.aibaodan.cn

[S24] C：获取本地时间
来源：http://rso.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xqw.0kj1m.cn

[S25] C：内存拷贝
来源：http://onn.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://tzg.zhengqikj.top

[S26] C：内存清零
来源：http://btm.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://drj.aibaodan.cn

[S27] C：定义常量
来源：http://gsk.daria6918.cn

const double PI = 3.14159;
来源：http://oib.jiagoushi.top

[S28] C：静态变量
来源：http://gix.aibaodan.cn

static int counter = 0;
来源：http://yef.aizwys.cn

[S29] C：变参函数
来源：http://ejt.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wob.wangshuangyany.cn

[S30] C：头文件保护
来源：http://tpu.yj20258.top

#ifndef X_H
来源：http://chh.daria6918.cn

#define X_H
来源：http://tzk.shanyushiyangkeji.top

#endif
来源：http://opy.zhiwuduotai.top

[S31] C++：Hello World
来源：http://eql.pengpengdd.cyou

#include <iostream>
来源：http://llh.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://vgv.52xcode.cn

[S32] C++：字符串
来源：http://hwi.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://shi.ehwqpu.com

[S33] C++：vector 增删
来源：http://enr.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pwb.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://dsr.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rvx.kuanghao11.cn

[S35] C++：map
来源：http://jur.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fkv.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://zyi.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zka.zhijiandao.cn

[S37] C++：set
来源：http://vhi.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqo.epnwcf.com

[S38] C++：排序
来源：http://xsg.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://zgv.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://tay.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jyp.shzxlz.cn

[S40] C++：查找元素
来源：http://zui.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ann.haohaochexian.top

[S41] C++：类与构造函数
来源：http://qsn.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://izr.zycfv.cn

[S42] C++：继承与虚函数
来源：http://dtu.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://kvl.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://zgs.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://vgz.aibaodan.cn

[S44] C++：引用传参
来源：http://cow.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://seo.yvedp.cn

[S45] C++：lambda
来源：http://yyp.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://bbx.yuxming.cn

[S46] C++：函数模板
来源：http://ile.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://otr.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://ncc.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hel.jinqigufen.top

[S48] C++：逐行读文件
来源：http://dmj.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gtr.ppjwa.cn


<!-- 参考信息 -->