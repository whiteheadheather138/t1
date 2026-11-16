代发 wailian999

[Q65] 回滚事务
来源：http://loe.zhiwuduotai.top

ROLLBACK;
来源：http://laj.tarul.cn

[Q66] 行锁查询
来源：http://iif.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://psf.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://ewx.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fgw.nanxinkj.top

[Q68] 保存点
来源：http://pbx.sjlbkw.cn

SAVEPOINT sp1;
来源：http://ulm.yuanzhike.top

ROLLBACK TO sp1;
来源：http://xgi.vehdjk.com

[Q69] 查看执行计划
来源：http://yib.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vvs.bbcook.cn

[Q70] 更新统计信息
来源：http://lhf.redwolf501.top

ANALYZE TABLE users;
来源：http://tbu.cqqwz.cn

[Q71] 查看建表语句
来源：http://cax.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lhn.hesvh.cn

[Q72] 查看索引
来源：http://xpz.mhx1999.top

SHOW INDEX FROM users;
来源：http://gpr.ydjk.org.cn

[Q73] 查看表状态
来源：http://vrq.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mds.jqgfzy.top

[Q74] 强制使用索引
来源：http://efo.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mkr.birdmap.top

[Q75] 日期格式化
来源：http://trs.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zez.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zph.jiagoushi.top

[Q76] 按天统计
来源：http://gvx.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lsj.fzhhl.top

[Q77] 时间加减
来源：http://mge.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhg.dashuyun.cn

[Q78] 当前时间
来源：http://oxu.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvh.andypj.xyz

[Q79] 字符串拼接
来源：http://dak.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yuk.andypj.xyz

[Q80] 字符串截取
来源：http://nke.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hmf.fengsongda.top

[Q81] 字符串替换
来源：http://ykn.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ofe.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://ycm.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wtt.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://zft.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://saq.shzxlz.cn

[Q84] 去除首尾空格
来源：http://pot.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://wyh.yj202588.top

[Q85] 数值取整
来源：http://jfi.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mww.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://hew.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pfn.52xcode.cn

[Q87] JSON 字段做条件
来源：http://jmv.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tub.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://fon.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tzq.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kuh.xinyue.icu

[Q89] 判断表是否存在
来源：http://iyz.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uer.sysykeji.top

[Q90] 生成序号列
来源：http://uam.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nuy.xuanzx.com

================================================================================
来源：http://ldw.zhiwuduotai.top

R. Bash 专题
来源：http://zng.snrcjt.cn

================================================================================
来源：http://yku.yueranfly.top

[R01] shebang 与严格模式
来源：http://niq.ivvv.top

#!/usr/bin/env bash
来源：http://ppu.zdbjq.cn

set -euo pipefail
来源：http://hwo.nwbrower.top

[R02] 变量赋值与使用
来源：http://khu.yj20258.top

name="Tom"; echo "$name"
来源：http://ryc.316326.xyz

[R03] 只读变量
来源：http://xwd.shuidangran.top

readonly PI=3.14
来源：http://aow.hnqzz.top

[R04] 位置参数
来源：http://sex.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bpw.redwolf501.top

[R05] 参数默认值
来源：http://dfs.zhengqikj.top

name="${1:-default}"
来源：http://mkm.daxiang520.top

[R06] 判断命令是否存在
来源：http://kox.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iic.cdnleiting.top

[R07] if 判断文件
来源：http://sae.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tqf.jinyuanbaomall.cn

[R08] 数值比较
来源：http://vvj.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gik.cqqwz.cn

[R09] 字符串比较
来源：http://cqb.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lqv.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://wvh.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eiu.yanxiufei.cn

[R11] case 多分支
来源：http://ysd.wangshuangyany.cn

case "$1" in
来源：http://lcq.hcnkem.com

start) echo "启动" ;;
来源：http://jdj.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://zun.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://tbl.yanxiufei.cn

esac
来源：http://ygc.shzxlz.cn

[R12] for 遍历文件
来源：http://ocd.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://kfg.yj202588.top

[R13] for 计数循环
来源：http://mqa.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://izy.nanxinkj.top

[R14] C 风格 for
来源：http://zhm.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ryf.jlsjyb.cn

[R15] while 逐行读文件
来源：http://hoo.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdx.gogol.net.cn

[R16] until 等待条件
来源：http://wuf.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ale.gotoacloud.top

[R17] 数组定义与取值
来源：http://qbv.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://xhq.gotoacloud.top

[R18] 遍历数组
来源：http://faj.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cvk.yvedp.cn

[R19] 数组长度
来源：http://nvr.sxryk.cn

echo "${#arr[@]}"
来源：http://xdr.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://vkc.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ztj.ctjpmb.com

[R21] 字符串长度
来源：http://vfo.jinyuanbaomall.cn

echo "${#s}"
来源：http://bal.zhoulong.xyz

[R22] 截取子串
来源：http://kds.yuanzhike.top

echo "${s:0:5}"
来源：http://ieb.sweek.top

[R23] 字符串替换
来源：http://ovc.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jta.meibo888.top

[R24] 大小写转换
来源：http://ezi.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ulb.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://tbm.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kxu.nwbrower.top

[R26] 命令替换
来源：http://ikq.meibo888.top

now=$(date +%F); echo "$now"
来源：http://vxa.hammf.cn

[R27] 算术展开
来源：http://cbq.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://vix.wangdashe.top

[R28] 浮点运算
来源：http://vmw.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://vrl.bjfxy.top

[R29] 定义函数
来源：http://kja.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hmn.wangdashe.top

[R30] 函数返回状态码
来源：http://hbk.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://fsf.hywenlv.cn

[R31] 局部变量
来源：http://hry.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://sun.chenzaomai.com

[R32] 参数个数校验
来源：http://kis.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gro.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://eay.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xrj.zhongyouzk.top

[R34] 退出时清理
来源：http://zry.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://zww.yonumen.top

[R35] 后台执行并等待
来源：http://bab.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hvq.cashguo.top

[R36] 并发执行多个任务
来源：http://dvg.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://puy.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://goe.yuxming.cn

files=$(ls -1)
来源：http://zti.jlsjyb.cn

[R38] 管道串联
来源：http://jkq.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://kuc.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://nzd.jianghu66.top

cmd > out.log 2>&1
来源：http://lif.birdmap.top

[R40] 追加写日志
来源：http://rej.hongshengwenyu.top

echo "log" >> out.log
来源：http://rzr.tanke756.top

[R41] 丢弃输出
来源：http://wyp.redwolf501.top

cmd >/dev/null 2>&1
来源：http://lyt.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://che.hongshengwenyu.top

wc -l < a.txt
来源：http://fxq.xuanzx.com

[R43] 按名字查找文件
来源：http://plu.haohaochexian.top

find . -name "*.log" -type f
来源：http://wah.haohaochexian.top

[R44] 按修改时间查找
来源：http://wto.sxryk.cn

find . -mtime -7 -type f
来源：http://cly.9152youxi.cn

[R45] 批量删除
来源：http://ujb.xylfe.cn

find . -name "*.tmp" -delete
来源：http://tqe.ivvv.top

[R46] 递归替换文件内容
来源：http://amp.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qmm.gogol.net.cn

[R47] sed 单行替换
来源：http://csn.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://nbm.chenzaomai.com

[R48] awk 取指定列
来源：http://yif.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://kmp.nwbrower.top

[R49] awk 带条件
来源：http://kcw.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jdm.zhijiandao.cn

[R50] awk 求和
来源：http://kip.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://obl.fehbvm.com

[R51] 排序去重取前几
来源：http://xwq.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wqf.zhaomingkeji.xyz

[R52] 统计行数
来源：http://mce.yuxming.cn

wc -l a.txt
来源：http://ogc.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://atm.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyo.ivvv.top

[R54] 比较两个文件
来源：http://gmw.pycfn.com

diff a.txt b.txt
来源：http://nqg.sufxvd.cn

[R55] 压缩与解压
来源：http://adh.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ibf.cucudq.cn

[R56] 远程拷贝
来源：http://uug.zhiwuduotai.top

scp file user@host:/path/
来源：http://ztb.cqqwz.cn

[R57] 远程执行命令
来源：http://oje.wangdashe.top

ssh user@host 'uptime'
来源：http://qzj.nanxuanxn.top

[R58] 下载文件
来源：http://jjo.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cwr.meibo888.top

[R59] 发 POST JSON
来源：http://vys.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tkh.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://bfv.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xue.bbcook.cn

[R61] 磁盘占用
来源：http://zmf.yueranfly.top

df -h;  du -sh *
来源：http://jwu.jinqigufen.top

[R62] 找最占空间的文件
来源：http://cok.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://ugu.tanke756.top

[R63] 内存与进程
来源：http://llb.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://gcb.chenzaomai.com

[R64] 结束进程
来源：http://iky.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://twn.aibaodan.cn

[R65] 查看端口占用
来源：http://fkh.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ymd.redwolf501.top

[R66] 定时任务
来源：http://ria.aizwys.cn

crontab -e;  crontab -l
来源：http://itd.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://kmi.jqgfzy.top

openssl rand -hex 16
来源：http://tmf.zycfv.cn

[R68] 计算文件校验值
来源：http://ues.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://bvy.xylfe.cn

[R69] 生成随机密码
来源：http://mdl.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://jxm.ppjwa.cn

[R70] 时间戳与互转
来源：http://pfn.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://vdt.shzxlz.cn

[R71] 日期格式化
来源：http://tvl.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://upo.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://pre.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ipc.hnqzz.top

[R73] 分割大日志
来源：http://hcy.guowangkeji.top

split -l 1000 big.log part_
来源：http://fty.hnxiangtu.top

[R74] 批量重命名
来源：http://ajt.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hsu.dashuyun.cn

[R75] 导出环境变量
来源：http://yny.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://jti.shangyingyoupin.top

[R76] 使用临时文件
来源：http://hku.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ate.jyoumei.cn

[R77] 读取用户输入
来源：http://oxs.sjlbkw.cn

read -rp "请输入: " ans
来源：http://bls.jqgufenzy.top

[R78] 交互式菜单
来源：http://lsx.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xxu.cqqwz.cn

[R79] 解析命令行选项
来源：http://xkp.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://swn.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://ivg.jinqigufen.top

time ./run.sh
来源：http://zch.sxryk.cn

================================================================================
来源：http://vpo.jqgfzy.top

S. C / C++ 专题
来源：http://qdg.xziqi.cn

================================================================================
来源：http://jhw.zdbjq.cn

[S01] C：Hello World
来源：http://jrl.shangyingyoupin.top

#include <stdio.h>
来源：http://csy.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tcp.daxiang520.top

[S02] C：变量与格式化输出
来源：http://zrx.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://jmx.316326.xyz

[S03] C：读入整数
来源：http://iqz.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://fkl.jlsjyb.cn

[S04] C：字符串复制
来源：http://jpl.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wjz.zdbjq.cn

[S05] C：字符串长度
来源：http://phv.c1oappe.top

strlen(s)
来源：http://qba.yj202588.top

[S06] C：字符串比较
来源：http://klq.cucudq.cn

strcmp(a, b) == 0
来源：http://mol.dianchejie.cn

[S07] C：数组遍历求和
来源：http://rqs.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xes.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://zkn.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iem.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://nbe.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://isg.daria6918.cn

[S10] C：指针与解引用
来源：http://poq.cashguo.top

int *p = &a;  *p = 5;
来源：http://xzu.nwbrower.top

[S11] C：逐行读文件
来源：http://vzp.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://yjg.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ehu.shanyushiyangkeji.top

fclose(f);
来源：http://grb.cqqwz.cn

[S12] C：写文件
来源：http://hvk.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rfk.cqqwz.cn

[S13] C：宏定义
来源：http://coo.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uhi.c1oappe.top

[S14] C：枚举
来源：http://yby.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://eki.yuanzhike.top

[S15] C：类型转换
来源：http://bem.daria6918.cn

(double) a / b
来源：http://vjw.vehdjk.com

[S16] C：位操作置位
来源：http://xcc.hnqzz.top

x |= (1 << 3);
来源：http://gla.yfazqb.com

[S17] C：安全拼接字符串
来源：http://vgj.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sye.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://tli.meibo888.top

int main(int argc, char **argv)
来源：http://wmi.hywenlv.cn

[S19] C：快速排序
来源：http://hmt.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pwk.chenzaomai.com

[S20] C：二分查找
来源：http://sgl.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://btd.yvedp.cn

[S21] C：字符类别判断
来源：http://skq.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zbs.tarul.cn

[S22] C：字符串转数字
来源：http://pom.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aim.quarkkingdee.top

[S23] C：随机数
来源：http://qxq.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oja.sxryk.cn

[S24] C：获取本地时间
来源：http://biu.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fjs.mhx1999.top

[S25] C：内存拷贝
来源：http://ldv.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://uji.fktsv.cn

[S26] C：内存清零
来源：http://zog.uphjek.com

memset(a, 0, sizeof a);
来源：http://fga.yanxiufei.cn

[S27] C：定义常量
来源：http://aqf.gaohongyu789.top

const double PI = 3.14159;
来源：http://bdw.shangyingyoupin.top

[S28] C：静态变量
来源：http://hhe.quarkkingdee.top

static int counter = 0;
来源：http://yxs.zhongyouzk.top

[S29] C：变参函数
来源：http://jxm.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ucs.jqgufenzy.top

[S30] C：头文件保护
来源：http://epg.svipenyu.cn

#ifndef X_H
来源：http://bqr.hesvh.cn

#define X_H
来源：http://orv.kuanghao11.cn

#endif
来源：http://sew.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://aum.zhoulong.xyz

#include <iostream>
来源：http://ank.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://suq.hammf.cn

[S32] C++：字符串
来源：http://vxr.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://lbz.bbcook.cn

[S33] C++：vector 增删
来源：http://odc.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hgu.yfazqb.com

[S34] C++：遍历 vector
来源：http://btz.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://cuk.316326.xyz


<!-- 参考信息 -->