代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jbo.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://qrw.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://seg.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wca.shzxlz.cn

[Q61] 移动平均
来源：http://bqm.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://whk.fengsongda.top

[Q62] 分组占比
来源：http://czi.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qsc.xuanzx.com

[Q63] 开启事务
来源：http://csi.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gwl.bbcook.cn

[Q64] 提交事务
来源：http://dij.gzhubu.top

COMMIT;
来源：http://dgy.vqdsnc.cn

[Q65] 回滚事务
来源：http://okm.zhijiandao.cn

ROLLBACK;
来源：http://kok.pycfn.com

[Q66] 行锁查询
来源：http://hfb.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://euy.52xcode.cn

[Q67] 设置隔离级别
来源：http://mcz.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sus.ivvv.top

[Q68] 保存点
来源：http://xva.yj20258.top

SAVEPOINT sp1;
来源：http://qvv.jyoumei.cn

ROLLBACK TO sp1;
来源：http://gax.daxiang520.top

[Q69] 查看执行计划
来源：http://kkd.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axn.andypj.xyz

[Q70] 更新统计信息
来源：http://uzb.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://qze.shuidangran.top

[Q71] 查看建表语句
来源：http://ikg.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fpm.zhoulong.xyz

[Q72] 查看索引
来源：http://ezy.haohaochexian.top

SHOW INDEX FROM users;
来源：http://kns.zdqjudy.top

[Q73] 查看表状态
来源：http://crx.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://izm.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://oex.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebm.jqgfzy.top

[Q75] 日期格式化
来源：http://nzf.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yyc.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hfd.gotoacloud.top

[Q76] 按天统计
来源：http://fps.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pah.feifeiyinyue.top

[Q77] 时间加减
来源：http://xcs.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uuu.shanyushiyangtech.top

[Q78] 当前时间
来源：http://gte.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cxs.c1oappe.top

[Q79] 字符串拼接
来源：http://fdr.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pdl.yj20258888.top

[Q80] 字符串截取
来源：http://iad.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://agc.xuanzx.com

[Q81] 字符串替换
来源：http://prq.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bdc.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://uea.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gua.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://szu.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uhh.yj20258888.top

[Q84] 去除首尾空格
来源：http://glj.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://ygb.chenjidiqi.icu

[Q85] 数值取整
来源：http://wym.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zsj.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://ppe.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hly.yfazqb.com

[Q87] JSON 字段做条件
来源：http://pue.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tre.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://rax.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://inr.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ozw.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://wcb.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://odg.xuanzx.com

[Q90] 生成序号列
来源：http://yme.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mcm.andypj.xyz

================================================================================
来源：http://xyt.zhijiandao.cn

R. Bash 专题
来源：http://nul.bbcook.cn

================================================================================
来源：http://vkr.316326.xyz

[R01] shebang 与严格模式
来源：http://rfz.jinqigufen.top

#!/usr/bin/env bash
来源：http://dtf.kuanghao11.cn

set -euo pipefail
来源：http://ouh.fengsongda.top

[R02] 变量赋值与使用
来源：http://axz.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://vhi.xuanzx.com

[R03] 只读变量
来源：http://uut.daxiang520.top

readonly PI=3.14
来源：http://tfu.ehwqpu.com

[R04] 位置参数
来源：http://phg.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhf.zhongyouzk.top

[R05] 参数默认值
来源：http://dic.birdmap.top

name="${1:-default}"
来源：http://gzu.9152youxi.cn

[R06] 判断命令是否存在
来源：http://rzq.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lfc.shanyushiyangtech.top

[R07] if 判断文件
来源：http://cpo.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qmg.yongpay.top

[R08] 数值比较
来源：http://nsd.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ggd.cdnleiting.top

[R09] 字符串比较
来源：http://sls.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://umw.xinyue.icu

[R10] 正则匹配
来源：http://xky.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nmr.yvedp.cn

[R11] case 多分支
来源：http://dnk.sysykeji.top

case "$1" in
来源：http://npj.yvedp.cn

start) echo "启动" ;;
来源：http://ttk.ybcxt.top

stop)  echo "停止" ;;
来源：http://nxf.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://fbs.cashguo.top

esac
来源：http://okw.yfazqb.com

[R12] for 遍历文件
来源：http://yny.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://kdr.sjlbkw.cn

[R13] for 计数循环
来源：http://ffl.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://spe.ehwqpu.com

[R14] C 风格 for
来源：http://mly.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dzp.yongpay.top

[R15] while 逐行读文件
来源：http://pcl.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gpy.svipenyu.cn

[R16] until 等待条件
来源：http://zho.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wrk.zhengqikj.top

[R17] 数组定义与取值
来源：http://pht.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://rxp.mhx1999.top

[R18] 遍历数组
来源：http://swb.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zwe.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://yyk.svipenyu.cn

echo "${#arr[@]}"
来源：http://snp.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://hgl.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://amf.fanxiaobao.xyz

[R21] 字符串长度
来源：http://hbp.fanxiaobao.xyz

echo "${#s}"
来源：http://xbx.sjlbkw.cn

[R22] 截取子串
来源：http://pvo.smart0.xyz

echo "${s:0:5}"
来源：http://jrt.jiagoushi.top

[R23] 字符串替换
来源：http://oxi.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nhg.andypj.xyz

[R24] 大小写转换
来源：http://xqi.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://tux.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://uui.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xhj.zhixingplan.top

[R26] 命令替换
来源：http://gcy.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://slk.hfpthk.cn

[R27] 算术展开
来源：http://sim.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://nkk.gzhubu.top

[R28] 浮点运算
来源：http://yqg.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://plg.dashuyun.cn

[R29] 定义函数
来源：http://yta.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vyq.ybcxt.top

[R30] 函数返回状态码
来源：http://dqj.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://xas.gotoacloud.top

[R31] 局部变量
来源：http://ljb.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://emj.shangyingyoupin.top

[R32] 参数个数校验
来源：http://wxc.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aht.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://buq.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zqb.xylfe.cn

[R34] 退出时清理
来源：http://mvq.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nrd.ydjk.org.cn

[R35] 后台执行并等待
来源：http://uro.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yri.yangfankeji.com

[R36] 并发执行多个任务
来源：http://zud.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://laa.ydzc1.top

[R37] 把输出赋给变量
来源：http://vqk.jinghuilouyu.cn

files=$(ls -1)
来源：http://jqy.shzxlz.cn

[R38] 管道串联
来源：http://uwg.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://eck.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://txg.fehbvm.com

cmd > out.log 2>&1
来源：http://oor.epnwcf.com

[R40] 追加写日志
来源：http://zvi.zhengqikj.top

echo "log" >> out.log
来源：http://pxe.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://qxb.sxryk.cn

cmd >/dev/null 2>&1
来源：http://eqc.yangfankeji.com

[R42] 输入重定向
来源：http://bel.dianchejie.cn

wc -l < a.txt
来源：http://yut.sufxvd.cn

[R43] 按名字查找文件
来源：http://hds.gogol.net.cn

find . -name "*.log" -type f
来源：http://oky.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://vcw.fengsongda.top

find . -mtime -7 -type f
来源：http://qke.nanxinkj.top

[R45] 批量删除
来源：http://drj.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://syz.nwbrower.top

[R46] 递归替换文件内容
来源：http://pvm.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hpp.birdmap.top

[R47] sed 单行替换
来源：http://mst.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://eqd.yanxiufei.cn

[R48] awk 取指定列
来源：http://ouh.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://fvs.hnqzz.top

[R49] awk 带条件
来源：http://dtp.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ufj.wangshuangyany.cn

[R50] awk 求和
来源：http://njd.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://dgk.quarkkingdee.top

[R51] 排序去重取前几
来源：http://hpe.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://awy.hnxiangtu.top

[R52] 统计行数
来源：http://gse.yanxiufei.cn

wc -l a.txt
来源：http://exq.pycfn.com

[R53] 查看文件头与实时尾
来源：http://nhx.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zsu.hongshengwenyu.top

[R54] 比较两个文件
来源：http://qwi.jinqigfzy.top

diff a.txt b.txt
来源：http://lgd.redwolf501.top

[R55] 压缩与解压
来源：http://tlq.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jfn.epnwcf.com

[R56] 远程拷贝
来源：http://akl.yj202588.top

scp file user@host:/path/
来源：http://cxq.ppjwa.cn

[R57] 远程执行命令
来源：http://ncy.gzhubu.top

ssh user@host 'uptime'
来源：http://bhx.hcnkem.com

[R58] 下载文件
来源：http://afu.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uua.redwolf501.top

[R59] 发 POST JSON
来源：http://ooq.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ckw.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://bgn.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://izo.zhongyouzk.top

[R61] 磁盘占用
来源：http://aly.meibo888.top

df -h;  du -sh *
来源：http://uiw.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://ptz.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://anh.yvedp.cn

[R63] 内存与进程
来源：http://rhd.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://eru.guannengcc.top

[R64] 结束进程
来源：http://azi.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://pdn.316326.xyz

[R65] 查看端口占用
来源：http://enp.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zuu.meibo888.top

[R66] 定时任务
来源：http://afz.birdmap.top

crontab -e;  crontab -l
来源：http://rht.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://usf.shanyushiyangtech.top

openssl rand -hex 16
来源：http://ukc.meibo888.top

[R68] 计算文件校验值
来源：http://iwh.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xed.meibo888.top

[R69] 生成随机密码
来源：http://ejw.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://cnl.zdbjq.cn

[R70] 时间戳与互转
来源：http://tyn.sweek.top

date +%s;  date -d @1700000000
来源：http://elz.hysaishi.cn

[R71] 日期格式化
来源：http://mll.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kgl.jqgfzy.top

[R72] 等待端口就绪
来源：http://uoy.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kft.jqgufenzy.top

[R73] 分割大日志
来源：http://ccu.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://iak.gogol.net.cn

[R74] 批量重命名
来源：http://wnh.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://woh.hnqzz.top

[R75] 导出环境变量
来源：http://sts.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://owq.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://sec.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmo.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://rlj.jiagoushi.top

read -rp "请输入: " ans
来源：http://esu.xinyue.icu

[R78] 交互式菜单
来源：http://xxe.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fny.haohaochexian.top

[R79] 解析命令行选项
来源：http://djs.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kat.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://gjm.snrcjt.cn

time ./run.sh
来源：http://uad.fanxiaobao.xyz

================================================================================
来源：http://mqi.hammf.cn

S. C / C++ 专题
来源：http://ckm.jlsjyb.cn

================================================================================
来源：http://yur.vehdjk.com

[S01] C：Hello World
来源：http://ivj.shuidangran.top

#include <stdio.h>
来源：http://mxl.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hfc.epnwcf.com

[S02] C：变量与格式化输出
来源：http://wbv.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://ttm.52xcode.cn

[S03] C：读入整数
来源：http://qkn.0kj1m.cn

int x; scanf("%d", &x);
来源：http://gyb.chenzaomai.com

[S04] C：字符串复制
来源：http://tci.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://xbu.ydzc1.top

[S05] C：字符串长度
来源：http://tzd.yj20258.top

strlen(s)
来源：http://uli.ehwqpu.com

[S06] C：字符串比较
来源：http://sgq.zycfv.cn

strcmp(a, b) == 0
来源：http://uap.uphjek.com

[S07] C：数组遍历求和
来源：http://mfs.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://miz.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://xlo.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://arc.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://sun.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mpg.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://blx.havefunace.top

int *p = &a;  *p = 5;
来源：http://arn.nwbrower.top

[S11] C：逐行读文件
来源：http://zss.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://rwo.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://thn.yonumen.top

fclose(f);
来源：http://lzj.kuanghao11.cn

[S12] C：写文件
来源：http://nrt.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://suj.pengpengdd.cyou

[S13] C：宏定义
来源：http://pko.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rsx.mhx1999.top

[S14] C：枚举
来源：http://wdr.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://bny.bbcook.cn

[S15] C：类型转换
来源：http://xin.gzhubu.top

(double) a / b
来源：http://png.9152youxi.cn

[S16] C：位操作置位
来源：http://bbs.hnxiangtu.top

x |= (1 << 3);
来源：http://wnt.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://dab.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fps.guowangkeji.top

[S18] C：命令行参数
来源：http://sut.uphjek.com

int main(int argc, char **argv)
来源：http://qyp.hywenlv.cn

[S19] C：快速排序
来源：http://pwp.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mfu.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://eda.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nri.nanxuanxn.top

[S21] C：字符类别判断
来源：http://zsi.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kqh.nanxuanxn.top

[S22] C：字符串转数字
来源：http://gnj.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rdq.shangyingyoupin.top

[S23] C：随机数
来源：http://grn.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pvq.fktsv.cn

[S24] C：获取本地时间
来源：http://rqe.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fef.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://tcv.xziqi.cn

memcpy(dst, src, n);
来源：http://vfc.sufxvd.cn

[S26] C：内存清零
来源：http://ctd.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://hwk.hnqzz.top

[S27] C：定义常量
来源：http://mka.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://zeg.jyoumei.cn

[S28] C：静态变量
来源：http://ogw.yj20258.top

static int counter = 0;
来源：http://ufl.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://thl.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ply.xuanzx.com

[S30] C：头文件保护
来源：http://gue.zhengqikj.top


<!-- 参考信息 -->