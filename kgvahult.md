代发 wailian999

SHOW INDEX FROM users;
来源：http://pmr.chenlongwang.top

[Q73] 查看表状态
来源：http://thi.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gcb.aizwys.cn

[Q74] 强制使用索引
来源：http://mvx.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mny.vehdjk.com

[Q75] 日期格式化
来源：http://yvp.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cqo.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tfo.ehwqpu.com

[Q76] 按天统计
来源：http://qzf.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sbn.daria6918.cn

[Q77] 时间加减
来源：http://rkt.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mjp.9152youxi.cn

[Q78] 当前时间
来源：http://abl.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://coe.nanxinkj.top

[Q79] 字符串拼接
来源：http://vul.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bvf.quarkkingdee.top

[Q80] 字符串截取
来源：http://yuv.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://don.ehwqpu.com

[Q81] 字符串替换
来源：http://cso.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jbz.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://neq.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://boi.birdmap.top

[Q83] 大小写转换
来源：http://wmk.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mmx.mhx1999.top

[Q84] 去除首尾空格
来源：http://ual.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://bzh.zhongyouzk.top

[Q85] 数值取整
来源：http://dic.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mjg.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://wio.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yej.ydzc1.top

[Q87] JSON 字段做条件
来源：http://jjw.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ydr.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://wfl.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://suv.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eej.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://rrt.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hth.cucudq.cn

[Q90] 生成序号列
来源：http://qul.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sxl.zhijiandao.cn

================================================================================
来源：http://vpg.sufxvd.cn

R. Bash 专题
来源：http://jct.zdqjudy.top

================================================================================
来源：http://kdw.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://rub.zdqjudy.top

#!/usr/bin/env bash
来源：http://qvh.tian-w.cn

set -euo pipefail
来源：http://kqb.vehdjk.com

[R02] 变量赋值与使用
来源：http://lsx.hcnkem.com

name="Tom"; echo "$name"
来源：http://qih.yanxiufei.cn

[R03] 只读变量
来源：http://shm.jqgfzy.top

readonly PI=3.14
来源：http://hzu.quarkkingdee.top

[R04] 位置参数
来源：http://lgo.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ehc.shanyushiyangtech.top

[R05] 参数默认值
来源：http://rlq.aibaodan.cn

name="${1:-default}"
来源：http://cvs.redwolf501.top

[R06] 判断命令是否存在
来源：http://anb.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gvi.yuxming.cn

[R07] if 判断文件
来源：http://ded.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mgj.chenzaomai.com

[R08] 数值比较
来源：http://ufc.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xsq.guannengcc.top

[R09] 字符串比较
来源：http://yek.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bld.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://rmn.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://szz.yfazqb.com

[R11] case 多分支
来源：http://qwv.gotoacloud.top

case "$1" in
来源：http://fjt.hnqzz.top

start) echo "启动" ;;
来源：http://rno.zhixingplan.top

stop)  echo "停止" ;;
来源：http://bnn.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://ghc.fehbvm.com

esac
来源：http://ses.xuanzx.com

[R12] for 遍历文件
来源：http://fth.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://ias.fktsv.cn

[R13] for 计数循环
来源：http://xvl.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://pqf.bbcook.cn

[R14] C 风格 for
来源：http://eyg.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nnp.cqqwz.cn

[R15] while 逐行读文件
来源：http://nya.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vlq.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://pmd.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ahv.aibaodan.cn

[R17] 数组定义与取值
来源：http://zzz.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://svx.dashuyun.cn

[R18] 遍历数组
来源：http://qij.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://osr.hesvh.cn

[R19] 数组长度
来源：http://ptt.tianlin.xyz

echo "${#arr[@]}"
来源：http://vay.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://nei.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xbp.xinyue.icu

[R21] 字符串长度
来源：http://uju.yonumen.top

echo "${#s}"
来源：http://ddi.jinqigufen.top

[R22] 截取子串
来源：http://rud.dashuyun.cn

echo "${s:0:5}"
来源：http://xnc.ydjk.org.cn

[R23] 字符串替换
来源：http://ugc.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mqe.daxiang520.top

[R24] 大小写转换
来源：http://luw.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dsw.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://shs.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xqy.sysykeji.top

[R26] 命令替换
来源：http://axa.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://ybh.iojbl.cn

[R27] 算术展开
来源：http://bwc.ybcxt.top

echo $((1 + 2 * 3))
来源：http://cah.sjlbkw.cn

[R28] 浮点运算
来源：http://iho.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://jfl.jlsjyb.cn

[R29] 定义函数
来源：http://sva.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hor.dashuyun.cn

[R30] 函数返回状态码
来源：http://ttt.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://zer.quarkkingdee.top

[R31] 局部变量
来源：http://tmr.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://lcj.ehwqpu.com

[R32] 参数个数校验
来源：http://gjv.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://npf.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://new.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dso.gzhubu.top

[R34] 退出时清理
来源：http://mjr.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://mds.zdbjq.cn

[R35] 后台执行并等待
来源：http://rrw.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dcs.yuanzhike.top

[R36] 并发执行多个任务
来源：http://pfv.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aak.snrcjt.cn

[R37] 把输出赋给变量
来源：http://zth.ctjpmb.com

files=$(ls -1)
来源：http://jay.tarul.cn

[R38] 管道串联
来源：http://pzb.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://xnt.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://cxx.316326.xyz

cmd > out.log 2>&1
来源：http://cxh.andypj.xyz

[R40] 追加写日志
来源：http://txg.nwbrower.top

echo "log" >> out.log
来源：http://urd.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://wjw.fzhhl.top

cmd >/dev/null 2>&1
来源：http://vaw.feifeiyinyue.top

[R42] 输入重定向
来源：http://jet.pycfn.com

wc -l < a.txt
来源：http://ytg.ctjpmb.com

[R43] 按名字查找文件
来源：http://mpu.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://xql.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://lpw.hnxiangtu.top

find . -mtime -7 -type f
来源：http://rnz.hnqzz.top

[R45] 批量删除
来源：http://pou.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://dxx.hesvh.cn

[R46] 递归替换文件内容
来源：http://tgc.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zsz.aibaodan.cn

[R47] sed 单行替换
来源：http://tzt.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tzu.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://ojh.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://cwv.havefunace.top

[R49] awk 带条件
来源：http://qjy.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ubl.hywenlv.cn

[R50] awk 求和
来源：http://elw.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://elg.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://gaj.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://zht.zycfv.cn

[R52] 统计行数
来源：http://jzf.sxryk.cn

wc -l a.txt
来源：http://osg.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://uqr.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wgv.xylfe.cn

[R54] 比较两个文件
来源：http://bkn.zycfv.cn

diff a.txt b.txt
来源：http://uxd.gzhubu.top

[R55] 压缩与解压
来源：http://xrz.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rik.gogol.net.cn

[R56] 远程拷贝
来源：http://utd.yangfankeji.com

scp file user@host:/path/
来源：http://qaf.smart0.xyz

[R57] 远程执行命令
来源：http://ydj.cqqwz.cn

ssh user@host 'uptime'
来源：http://rkr.fanxiaobao.xyz

[R58] 下载文件
来源：http://iki.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hom.svipenyu.cn

[R59] 发 POST JSON
来源：http://xuc.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fms.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://iwo.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bnb.yonumen.top

[R61] 磁盘占用
来源：http://eki.sufxvd.cn

df -h;  du -sh *
来源：http://pcq.ctjpmb.com

[R62] 找最占空间的文件
来源：http://crn.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://ffj.c1oappe.top

[R63] 内存与进程
来源：http://tzh.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://bff.jinqigufen.top

[R64] 结束进程
来源：http://foc.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://xrm.shuidangran.top

[R65] 查看端口占用
来源：http://wak.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xwn.hysaishi.cn

[R66] 定时任务
来源：http://ruz.zdqjudy.top

crontab -e;  crontab -l
来源：http://xdg.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://eul.yuxming.cn

openssl rand -hex 16
来源：http://aoy.yvedp.cn

[R68] 计算文件校验值
来源：http://gbh.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jog.jinqigufen.top

[R69] 生成随机密码
来源：http://zpd.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://xsj.yongpay.top

[R70] 时间戳与互转
来源：http://kjy.hcnkem.com

date +%s;  date -d @1700000000
来源：http://qgn.wangdashe.top

[R71] 日期格式化
来源：http://uuh.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://inl.jiagoushi.top

[R72] 等待端口就绪
来源：http://xyr.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xao.redwolf501.top

[R73] 分割大日志
来源：http://kpf.andypj.xyz

split -l 1000 big.log part_
来源：http://mwl.cheryme.top

[R74] 批量重命名
来源：http://rkr.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnb.zycfv.cn

[R75] 导出环境变量
来源：http://sof.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://qus.zdqjudy.top

[R76] 使用临时文件
来源：http://wxh.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xcr.ehwqpu.com

[R77] 读取用户输入
来源：http://gtv.zhongyouzk.top

read -rp "请输入: " ans
来源：http://gkd.yanxiufei.cn

[R78] 交互式菜单
来源：http://ovi.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jtk.dianchejie.cn

[R79] 解析命令行选项
来源：http://ssv.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ztx.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://zbd.guannengcc.top

time ./run.sh
来源：http://fgk.hysaishi.cn

================================================================================
来源：http://fnc.zhongyouzk.top

S. C / C++ 专题
来源：http://bbn.yuxming.cn

================================================================================
来源：http://zhv.zdqjudy.top

[S01] C：Hello World
来源：http://jhr.snrcjt.cn

#include <stdio.h>
来源：http://hem.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xen.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://ukf.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://rsi.ydjk.org.cn

[S03] C：读入整数
来源：http://nea.aizwys.cn

int x; scanf("%d", &x);
来源：http://hgv.daxiang520.top

[S04] C：字符串复制
来源：http://nxd.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://zza.hnxiangtu.top

[S05] C：字符串长度
来源：http://ksm.mhx1999.top

strlen(s)
来源：http://ygb.fehbvm.com

[S06] C：字符串比较
来源：http://xkf.yonumen.top

strcmp(a, b) == 0
来源：http://iuf.tian-w.cn

[S07] C：数组遍历求和
来源：http://cqg.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sxa.tanke756.top

[S08] C：动态内存分配与释放
来源：http://flf.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dvz.uphjek.com

[S09] C：结构体定义与初始化
来源：http://rhz.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dfj.zhijiandao.cn

[S10] C：指针与解引用
来源：http://nno.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://iqw.pycfn.com

[S11] C：逐行读文件
来源：http://lvh.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://ery.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jtl.bbcook.cn

fclose(f);
来源：http://pop.jiagoushi.top

[S12] C：写文件
来源：http://alo.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fkw.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://rkc.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cgz.ywan-chungtsiang.top

[S14] C：枚举
来源：http://eij.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fvz.meibo888.top

[S15] C：类型转换
来源：http://zbj.cdnleiting.top

(double) a / b
来源：http://vag.zhongyouzk.top

[S16] C：位操作置位
来源：http://ylc.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://nbi.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://ggc.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://for.zhixingplan.top

[S18] C：命令行参数
来源：http://lfl.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://gho.hongshengwenyu.top

[S19] C：快速排序
来源：http://gbb.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://sof.tanke756.top

[S20] C：二分查找
来源：http://bfp.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dey.xziqi.cn

[S21] C：字符类别判断
来源：http://cka.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sfr.yj202588.top

[S22] C：字符串转数字
来源：http://gnf.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://twy.haohaochexian.top

[S23] C：随机数
来源：http://fwz.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jfm.yj202588.top

[S24] C：获取本地时间
来源：http://wrq.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sti.cheryme.top

[S25] C：内存拷贝
来源：http://gse.hammf.cn

memcpy(dst, src, n);
来源：http://jno.cheryme.top

[S26] C：内存清零
来源：http://fnu.ydzc1.top

memset(a, 0, sizeof a);
来源：http://xhe.jqgufenzy.top

[S27] C：定义常量
来源：http://rdj.chenlongwang.top

const double PI = 3.14159;
来源：http://frv.hnqzz.top

[S28] C：静态变量
来源：http://jmc.jinyuanbaomall.cn

static int counter = 0;
来源：http://dwe.andypj.xyz

[S29] C：变参函数
来源：http://bgj.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jkc.cashguo.top

[S30] C：头文件保护
来源：http://crw.ydzc1.top

#ifndef X_H
来源：http://grm.nanxuanxn.top

#define X_H
来源：http://kgd.yuanzhike.top

#endif
来源：http://jyn.daxiang520.top

[S31] C++：Hello World
来源：http://gko.xingfuxueyuan.xyz

#include <iostream>
来源：http://wih.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://ahp.smart0.xyz

[S32] C++：字符串
来源：http://qdu.ivvv.top

std::string s = "hi";  s += "!";
来源：http://tzg.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://kxu.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pwg.hesvh.cn

[S34] C++：遍历 vector
来源：http://lkc.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://jih.svipenyu.cn

[S35] C++：map
来源：http://ocf.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fho.sweek.top

[S36] C++：unordered_map
来源：http://ibe.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jyd.cdnleiting.top

[S37] C++：set
来源：http://nyl.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yys.hnqzz.top

[S38] C++：排序
来源：http://elr.tanke756.top

std::sort(v.begin(), v.end());
来源：http://bkf.tanke756.top

[S39] C++：自定义比较器排序
来源：http://met.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gth.redwolf501.top

[S40] C++：查找元素
来源：http://tam.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fth.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://mih.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ndd.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://rzi.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://qzc.bbcook.cn


<!-- 参考信息 -->